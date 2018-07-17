# Information on the Open Watch Project
Project OpenWatch is the initiative undertaken by BLOCKS, who came into the limelight for their modular smartwatch. The goal of this initiative is to make a fully open source OS so any smartwatch that can have AOSP builds or be ported to AOSP can have a fully functional Watch OS.

Here is a link to see our current to-do, in progress, done list https://goo.gl/62UnLw

# Build android 8.1 for Harmony (Various mt6580 smartwatches)

Kingwear makes a reference board that they use in their own products and has sold it to multiple diffrent manufacturers

List of confirmed working devices (Probably more out there):
* Kingwear KW88, KW98, KW99
* Blocks Watch
* Look Watch
* Zeblaze Thor, Thor S
* Lemfo LES1
* IQ I2
* Diggro DI01, DI07

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

repopick 220036 219443 220034 220285 220286 220287 220288 220293 220442
