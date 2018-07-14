# Build lineage 15.1 for mt6580 watches

## Local manifest
```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="openwatchproject/android_device_mediatek_8gb" path="device/mediatek/8gb" remote="github" revision="android-8.1" />
  <project name="openwatchproject/android_device_mediatek_mt6580-common" path="device/mediatek/mt6580-common" remote="github" revision="android-8.1" />
  <project name="openwatchproject/android_kernel_mediatek_mt6580" path="kernel/mediatek/mt6580" remote="github" revision="lineage-15.1" />
  <project name="openwatchproject/android_vendor_mediatek_mt6580-common" path="vendor/mediatek/mt6580-common" remote="github" revision="android-8.0" />
</manifest>
```

## Requried patch list
https://review.lineageos.org/#/c/220036 # fw/av mtk

https://review.lineageos.org/#/c/219443 # earlysuspend

https://review.lineageos.org/#/c/220034 # mtk flag
