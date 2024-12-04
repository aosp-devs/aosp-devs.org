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

BayLibre have support packages for

* MediaTek Genio 350-EVK: [https://baylibre.pages.baylibre.com/mediatek/rita/device/mediatek/boards/mtk-android-14/index.html](https://baylibre.pages.baylibre.com/mediatek/rita/device/mediatek/boards/mtk-android-14/index.html)
* Texas Instruments AM62X and AM62PX: [https://baylibre.pages.baylibre.com/ti/android/doc/ti-android-15/index.html](https://baylibre.pages.baylibre.com/ti/android/doc/ti-android-15/index.html)

Other projects:

* Generic Qualcomm SDM845 device support: [https://github.com/aospm/android_device_generic_sdm845](https://github.com/aospm/android_device_generic_sdm845)
  - support for several handsets based on the SDM845

## Generic HALs

* drm_hwcomposer [https://gitlab.freedesktop.org/drm-hwcomposer/drm-hwcomposer](https://gitlab.freedesktop.org/drm-hwcomposer/drm-hwcomposer) - DRM/KMS based HWComposer implementation used on many devices
* Force Feedback haptics hal: [https://github.com/aospm/external_vibrator-ff](https://github.com/aospm/external_vibrator-ff) - A generic haptics HAL which supports drivers using the force feedback API via input class devices.
* TinyHAL audio HAL: [https://github.com/CirrusLogic/tinyhal](https://github.com/CirrusLogic/tinyhal) - Generic Audio HAL on top of tinyalsa and tinycompress. Configured via XML
* Lights HAL: [https://github.com/SoMainline/android-lights-hal](https://github.com/SoMainline/android-lights-hal) - control for backlight and LEDs
* Keymaster/Gatekeeper on OP-TEE: [https://github.com/linaro-swg/kmgk](https://github.com/linaro-swg/kmgk)
* Camera: [https://libcamera.org/index.html](https://libcamera.org/index.html)

## Distros

* LineageOS: [https://lineageos.org/](https://lineageos.org/) - a free and open-source operating system for various devices, based on the Android mobile platform.
* Replicant: [https://replicant.us/](https://replicant.us/) - an attempt to get rid of all non-open components. While it has fallen far behind upstream, it has some interesting beginnings and starting points of open drivers and firmware
* GrapheneOS: [https://grapheneos.org/](https://grapheneos.org/) - Security and privacy minded AOSP fork for Pixel devices
* CalyxOS: [https://calyxos.org/](https://calyxos.org/) - Privacy minded fork of AOSP with MicroG support
* /e/ OS: [https://e.foundation/e-os/](https://e.foundation/e-os/) - Privacy minded LineageOS fork
* GloDroid: [https://glodroid.github.io/](https://glodroid.github.io/) - AOSP distro for Orange Pi and other boards
* Project Celadon: [https://projectceladon.github.io/celadon-documentation/getting-started/getting-started.html](https://projectceladon.github.io/celadon-documentation/getting-started/getting-started.html) - AOSP distro for Intel platforms, virtual machines and containers [source](https://github.com/projectceladon)

## Open Source apps that can replace functionality that exists in Android, but not AOSP

* [K-9 Mail](https://k9mail.app) - Free email app
* [Organic Maps](https://organicmaps.app) - Maps based on [OpenStreetMap](https://openstreetmap.org/) data
* [VLC](https://www.videolan.org/vlc/download-android.html) - Media player
* [Ungoogled Chromium](https://github.com/ungoogled-software/ungoogled-chromium) - Chromium without Google requirements
* [Forecastie](https://github.com/martykan/forecastie) - Weather applet
* [Lawnchair](https://lawnchair.app/) - Full-featured launcher resembling the Pixel launcher
* [MicroG](https://microg.org/) - Open, API and ABI compatible reimplementations of most GMS services
