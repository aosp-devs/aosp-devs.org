---
layout: default
---

There are many projects that extend AOSP in various ways. Here we divide them into:

* Board support: the code required to allow Android to run on a given board or
  family of boards
* Generic HALs: hardware support that applies to multiple boards
* Android distros: modifications to the Android framework and applications


## Board support

The Devboards for Android project [(https://devboardsforandroid.linaro.org/en/latest/](https://devboardsforandroid.linaro.org/en/latest/)
adds support to upstream AOSP for several boards including:

* Qualcomm® Robotics RB5 Development Kit
* RB3 Kit for DragonBoard 845c
* Khadas VIM3 / VIM3L
* Snapdragon(tm) 8 Gen 2 Mobile Hardware Development Kit (HDK 8550)
* Hikey 960

Baylibre have support packages for

* MediaTek MT8365 (i350): [https://baylibre.pages.baylibre.com/mediatek/rita/device/mediatek/boards/mtk-android-14/index.html](https://baylibre.pages.baylibre.com/mediatek/rita/device/mediatek/boards/mtk-android-14/index.html)
* Texas Instruments: [https://baylibre.pages.baylibre.com/ti/android/doc/ti-android-15/index.html](https://baylibre.pages.baylibre.com/ti/android/doc/ti-android-15/index.html)

Other projects:

Generic Qualcomm SDM845 device support: [https://github.com/aospm/android_device_generic_sdm845](https://github.com/aospm/android_device_generic_sdm845)
 - support for several handsets based on the SDM845


## Generic HALs

* drm_hwcomposer [https://gitlab.freedesktop.org/drm-hwcomposer/drm-hwcomposer](https://gitlab.freedesktop.org/drm-hwcomposer/drm-hwcomposer) - DRM/KMS based HWComposer implementation used on many devices
* Force Feedback haptics hal: [https://github.com/aospm/external_vibrator-ff](https://github.com/aospm/external_vibrator-ff) - A generic haptics HAL which supports drivers using the force feedback API via input class devices.
* TinyHAL audio HAL: [https://github.com/CirrusLogic/tinyhal](https://github.com/CirrusLogic/tinyhal) - Generic Audio HAL on top of tinyalsa and tinycompress. Configured via XML
* Lights HAL: [https://github.com/SoMainline/android-lights-hal](https://github.com/SoMainline/android-lights-hal) - control for backlight and LEDs
* Keymaster/Gatekeeper on OP-TEE: [https://github.com/linaro-swg/kmgk](https://github.com/linaro-swg/kmgk)
* Camera: [https://libcamera.org/index.html](https://libcamera.org/index.html)

## Distros

LineageOS: [https://lineageos.org/](https://lineageos.org/) - a free and open-source operating system for various devices, based on the Android mobile platform.

