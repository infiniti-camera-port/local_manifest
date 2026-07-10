# infiniti camera-port crDroid 16.0 manifest

This repository publishes the complete promoted crDroid v3 split graph for the
OnePlus 15 (`infiniti`). The local manifest selects all independent repositories
needed by the bring-up: 36 projects in total, made up of 26
`infiniti-camera-port/*` projects and 10 external closure projects. It also
contains 34 optional removals so it can safely replace either crDroid or
upstream OnePlus-SM8850 projects when present.

The promoted `infiniti` path has historical build and runtime evidence. The
macan, macanc, and fairlady variants have not yet been freshly built or
runtime-validated from this split graph. Their builds and static QA are queued
in the approved all-device pass; do not infer a result for them yet.

## Quick start

Install Google's `repo` launcher and Git LFS first, then start from an empty
directory:

```sh
git lfs install
git clone --depth=1 https://github.com/infiniti-camera-port/local_manifest.git
git clone --depth=1 https://github.com/infiniti-camera-port/patches.git
mkdir crdroid-16
cd crdroid-16

repo init --git-lfs \
  -u https://github.com/crdroidandroid/android.git \
  -b 16.0
mkdir -p .repo/local_manifests
cp ../local_manifest/local_manifests/infiniti-camera.xml \
  .repo/local_manifests/infiniti-camera.xml
repo sync -c --no-clone-bundle --no-tags -j8
```

Do not use `--force-sync` as a routine recovery step. If `repo sync` reports a
path collision or a dirty project, inspect that checkout before deciding how to
preserve or remove local work.

## Branch contract

Exactly these four shared common repositories use `16.0-infiniti`:

- `android_device_oneplus_sm8850-common`
- `vendor_oneplus_camera-sm8850-common`
- `proprietary_vendor_oneplus_sm8850-common`
- `proprietary_vendor_oneplus_camera-sm8850-common`

Every other `infiniti-camera-port/*` project in the manifest uses `16.0`. Do not
flatten the four common rows to `16.0`, and do not move the other rows onto the
common branch.

## Hydrate and verify proprietary inputs

After the sync, explicitly hydrate and verify the four LFS-backed proprietary
inputs used by the infiniti build:

```sh
for path in \
  proprietary/vendor/oneplus/camera-infiniti \
  proprietary/vendor/oneplus/camera-sm8850-common \
  vendor/oneplus/infiniti \
  vendor/oneplus/sm8850-common
do
  git -C "$path" lfs pull
  git -C "$path" lfs fsck
done
```

The LFS object service is `lfs.p0g.ca`. If it requests authentication, configure
credentials through a Git credential helper or a protected netrc file. Never
put credentials in this manifest, a committed config file, a command line, or
shell history.

## Apply the guarded build overlays and build

The promoted source changes are already in the manifest repositories. Manifest
consumers must not apply the portable `patch/` profile to this tree; it would
apply those source changes twice. Only apply the guarded crDroid build overlays
below.

```sh
python3 ../patches/build-patches/apply-build-patches.py \
  --repo-root "$PWD" --check-only

# Apply mode: the same runner without --check-only.
python3 ../patches/build-patches/apply-build-patches.py --repo-root "$PWD"

source build/envsetup.sh
lunch lineage_infiniti-bp4a-userdebug
NINJA_ARGS='-k 0' WITH_SU=true mka bacon
```

`--check-only` validates overlay state; it does not compile Android. Review its
report before running apply mode. The final command is the promoted build lane
used by this project.

## Patch consumers

This manifest points directly at the promoted organization repositories, where
the crDroid v3 changes are already present. The portable profile is only for
downstream trees that keep their original upstream project remotes instead of
consuming this manifest.
