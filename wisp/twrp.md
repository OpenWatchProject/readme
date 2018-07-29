# Build TWRP for wisp devices

Add to `.repo/local_manifests/wisp.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="OpenWatchProject/android_device_mediatek_wisp" path="device/mediatek/wisp" remote="github" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_wisp-eng
mka recoveryimage
```
