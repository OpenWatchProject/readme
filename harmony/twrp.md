# Build TWRP for harmony devices

Add to `.repo/local_manifests/harmony.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="OpenWatchProject/android_device_mediatek_harmony" path="device/mediatek/harmony" remote="github" revision="android-8.0" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_harmony-eng
mka recoveryimage
```
