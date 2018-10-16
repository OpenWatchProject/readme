# Build android 7.1 for platy  (ZTE Quartz)

## Local manifest
```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="openwatchproject/android_device_zte_platy" path="device/mediatek/harmony" remote="github" revision="cm-14.1" />
  <project name="openwatchproject/android_kernel_zte_msm8909w" path="kernel/zte/msm8909w" remote="github" revision="cm-14.1" />
  <project name="openwatchproject/android_vendor_zte_platy" path="vendor/zte/platy" remote="github" revision="cm-14.1" />
  <project name="openwatchproject/android_vendor_watch" path="vendor/watch" remote="github" revision="master" />
  <project name="openwatchproject/android_hardware_qcom_audio" path="hardware/qcom/audio-caf/msm8909" groups="qcom,qcom_audio" revision="cm-14.1-caf-8909" />
  <project name="openwatchproject/android_hardware_qcom_display" path="hardware/qcom/display-caf/msm8909" groups="pdk,qcom,qcom_display" revision="cm-14.1-caf-8909" />
  <project name="openwatchproject/android_hardware_qcom_media" path="hardware/qcom/media-caf/msm8909" groups="qcom" revision="cm-14.1-caf-8909" />
</manifest>
```

## Requried patch list
https://review.lineageos.org/#/c/231822 # Change BR_FAMILY to msm8909 instead of msm8916

If building Lineage-14.1 here is a repo pick command to grab all of these

repopick 231822
