# Build android 8.1 for Harmony (Various mt6580 smartwatches)

## Local manifest
```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="openwatchproject/android_device_mediatek_harmony" path="device/mediatek/harmony" remote="github" revision="android-8.1" />
  <project name="openwatchproject/android_kernel_mediatek_mt6580" path="kernel/mediatek/mt6580" remote="github" revision="android-8.1" />
  <project name="openwatchproject/android_vendor_mediatek_harmony" path="vendor/mediatek/harmony" remote="github" revision="android-8.1" />
</manifest>
```

## Requried patch list
https://review.lineageos.org/#/c/220036 # fw/av mtk

https://review.lineageos.org/#/c/219443 # earlysuspend

https://review.lineageos.org/#/c/220034 # mtk flag

https://review.lineageos.org/#/c/220285 # Disable fixed size

https://review.lineageos.org/#/c/220286 # Disable dashboard icons and summaries

https://review.lineageos.org/#/c/220287 # Change dashboard tile layout

https://review.lineageos.org/#/c/220288 # zygote whitelist

https://review.lineageos.org/#/c/220293 # Disable settings search bar

https://review.lineageos.org/#/c/220442 # Disable toolbar in settings

If building Lineage-15.1 here is a repo pick command to grab all of these