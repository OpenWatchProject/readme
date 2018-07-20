# Build TWRP for inharmony devices

Add to `.repo/local_manifests/infinity.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="OpenWatchProject/twrp_device_mediatek_infinity" path="device/mediatek/infinity" remote="github" revision="android-7.0" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_infinity-eng
mka recoveryimage
```
