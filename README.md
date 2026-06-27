# infiniti camera local manifest

Addendum to the `oneplus-sm8850-development/android` LineageOS manifest that re-points
the camera stack at the `infiniti-camera-port` org so you can build and test the camera
changes. The bring-up has landed on each repo's default branch.

## Use

After `repo init` from `oneplus-sm8850-development/android`:

```
cp local_manifests/infiniti-camera.xml .repo/local_manifests/
repo sync
```
