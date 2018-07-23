# Build TWRP for continuum devices

Add to `.repo/local_manifests/continuum.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="OpenWatchProject/android_device_mediatek_continuum" path="device/mediatek/continuum" remote="github" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_continuum-eng
mka recoveryimage
```
