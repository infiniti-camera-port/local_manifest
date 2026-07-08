# infiniti camera local manifest

Addendum for the crDroid staging build that re-points the camera stack at the
`infiniti-camera-port` org for infiniti, macan, macanc, and fairlady. Wave 2B
tracks only `staging/crdroid/v3`, with the single approved
`staging/crdroid/v3-infiniti` override for `android_device_oneplus_sm8850-common`.

## Use

After `repo init` from the crDroid Android manifest:

```
cp local_manifests/infiniti-camera.xml .repo/local_manifests/
repo sync
```

Default branch promotion is Marker-4 gated, so this manifest intentionally does
not track promoted default branches.
