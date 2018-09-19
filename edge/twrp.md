# Build TWRP for edge devices

Add to `.repo/local_manifests/edge.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="OpenWatchProject/android_device_mediatek_edge" path="device/mediatek/edge" remote="github" revision="android-7.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_edge-eng
mka recoveryimage
```
