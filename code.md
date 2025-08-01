---
layout: default
---

There are many projects that extend AOSP in various ways. Here we divide them into:

* Board support: the code required to allow Android to run on a given board or
  family of boards
* Generic HALs: hardware support that applies to multiple boards
* Android distros: modifications to the Android framework and applications
* Open source apps: apps that can replace functionality that exists in Android, but not AOSP

## Code search

To search the AOSP source code, you can use [Android Code Search](https://cs.android.com) provided by Google.

To see the differences between Android releases, you can use
[Android Open Source Project Changelogs](https://mikeng.github.io/aosp.changelog.to/)
provided by the [github repo](https://github.com/mikeNG/aosp.changelog.to).


## Board support

The Devboards for Android project [https://devboardsforandroid.linaro.org/en/latest/](https://devboardsforandroid.linaro.org/en/latest/)
adds support to upstream AOSP for several boards including:

* Qualcomm® Robotics RB5 Development Kit
* RB3 Kit for DragonBoard 845c
* Khadas VIM3 / VIM3L
* Snapdragon(tm) 8 Gen 2 Mobile Hardware Development Kit (HDK 8550)
* Hikey 960

BayLibre have support packages for:

* MediaTek Genio 700, 510 and 350 EVKs: [https://baylibre.pages.baylibre.com/mediatek/rita/device/mediatek](https://baylibre.pages.baylibre.com/mediatek/rita/device/mediatek)
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
* Projects by BlissLabs:
  * Waydroid: [https://waydro.id/](https://waydro.id/) - A container-based approach to boot a full Android system on regular GNU/Linux systems running Wayland based desktop environments.
  * BlissRoms: [https://blissroms.org/](https://blissroms.org/) - BlissRoms, an open-source operating system built upon Android Open Source Project, that offers a harmonious blend of customization, options, and security features.
  * BlissOS: [https://blissos.org/](https://blissos.org/) - An Android-based open source OS that incorporates many optimizations, features, and that supports many more devices. What's more? It's available for just about any Chromebook, PC or tablet released in the last 10 years.

## Open Source apps

* [K-9 Mail](https://k9mail.app) - Free email app
* [Organic Maps](https://organicmaps.app) - Maps based on [OpenStreetMap](https://openstreetmap.org/) data
* [VLC](https://www.videolan.org/vlc/download-android.html) - Media player
* [Ungoogled Chromium](https://github.com/ungoogled-software/ungoogled-chromium) - Chromium without Google requirements
* [Forecastie](https://github.com/martykan/forecastie) - Weather applet
* [Lawnchair](https://lawnchair.app/) - Full-featured launcher resembling the Pixel launcher
* [MicroG](https://microg.org/) - Open, API and ABI compatible reimplementations of most GMS services
 
## Android in Automotive

* [COVESA AOSP SDK](https://github.com/COVESA/covesa-aosp-sdk) - initiative to standardize vehicle interfaces for application developers. More about COVESA - [here](https://wiki.covesa.global/display/WIK4/Automotive+AOSP+App+Framework+Standardization+Expert+Group).
