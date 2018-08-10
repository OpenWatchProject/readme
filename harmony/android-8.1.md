# Build android 8.1 for Harmony (Various mt6580 smartwatches)

## Local manifest
```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="openwatchproject/android_device_mediatek_harmony" path="device/mediatek/harmony" remote="github" revision="android-8.1" />
  <project name="openwatchproject/android_kernel_mediatek_mt6580" path="kernel/mediatek/mt6580" remote="github" revision="android-8.1" />
  <project name="openwatchproject/android_vendor_mediatek_harmony" path="vendor/mediatek/harmony" remote="github" revision="android-8.1" />
  <project name="openwatchproject/android_vendor_watch" path="vendor/watch" remote="github" revision="master" />
  <project name="openwatchproject/android_packages_apps_WatchSettings" path="packages/apps/WatchSettings" remote="github" revision="lineage-15.1" />
</manifest>
```

## Requried patch list
https://review.lineageos.org/#/c/220036 # fw/av mtk

https://review.lineageos.org/#/c/219443 # earlysuspend

https://review.lineageos.org/#/c/220034 # mtk flag

https://review.lineageos.org/#/c/220288 # zygote whitelist

https://review.lineageos.org/#/c/220442 # Disable toolbar in settings

https://review.lineageos.org/#/c/220506 # DNM: temp bt changes

https://review.lineageos.org/#/c/220507 # Support IOS BLE pairing

https://review.lineageos.org/#/c/220508 # Support IOS BLE pairing

https://review.lineageos.org/#/c/220510 # DNM: support legacy mtk bt hals

https://review.lineageos.org/#/c/221654 # Disable restrictions on swipe to dismiss and ActionBars

https://review.lineageos.org/#/c/222237 # DMN: Add back atomic symbols

https://review.lineageos.org/#/c/221359 # LINEAGE ONLY?: lineageParts:Remove actionbar calls

https://review.lineageos.org/#/c/222344 # Overlay LatinIME for round-watch

https://review.lineageos.org/#/c/222346 # Overlay Calculator for round-watch

https://review.lineageos.org/#/c/222493 # Overlay layouts for round-watch (DeskClock)

https://review.lineageos.org/#/c/223332 # Update device default colors for darker UI

https://review.lineageos.org/#/c/223333 # Set windowElevation to 0 on watch dialogs

https://review.lineageos.org/#/c/223334 # Animation and style adjustments to make UI stutter go away

If building Lineage-15.1 here is a repo pick command to grab all of these

repopick 220036 219443 220034 220288 220442 220506 220507 220508 220510 221654 222237 221359 222344 222346 222493 223332 223333 223334

