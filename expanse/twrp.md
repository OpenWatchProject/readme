# Build TWRP for expanse devices

Add to `.repo/local_manifests/expanse.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="OpenWatchProject/android_device_mediatek_expanse" path="device/mediatek/expanse" remote="github" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_expanse-eng
mka recoveryimage
```
