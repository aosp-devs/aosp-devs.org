---
layout: post
excerpt_separator: <!--more-->
title:  "Pixel support dropped from Android 16: what it means for the AOSP developer community"
author: Chris Simmonds
---

Dropping Pixel support from Android 16 was a surprise. While the AOSP code base is still sufficient to build devices for new hardware, even without support from Google, it makes it harder because there is less reference code to show how the lower layers of the operating system are intended to work. Call to action: we can fill the gap by sharing the device knowledge that we have. That is exactly what we at [aosp-devs.org](https://aosp-devs.org) are here for

<!--more-->
 	 	

## A quiet change in the device/google/ directory
AOSP includes configurations for a range of hardware and emulated targets - you can find them in the device/ directory, with subdirectories organized by manufacturer. Device configuration in this context refers to the configuration files, build scripts, kernel sources and binary blobs that you need to compile and flash a working build. Up to Android 16 device/google contained configuration for the Nexus and Pixel devices that are currently in their support window. But in Android 16, device/google contains only configurations based on the Cuttlefish emulator.

Google confirmed that the omission is intentional. [Bill Ye posted the following](https://groups.google.com/g/android-building/c/c4_W34xH55I/m/Cu0jCJjtAwAJ) on the Android Building mail list

_"We remain committed to AOSP updates. You continue to have the option to build Cuttlefish and GSI targets from the sources for experimentation."_

Separately, [Seang Chau posted this on X](https://x.com/seangchau/status/1933029688202703062?t=Btky5f3cIU5qQQI14cf-VQ):

_"We're seeing some speculation that AOSP is being discontinued. To be clear, AOSP is NOT going away. AOSP was built on the foundation of being an open platform for device implementations, SoC vendors, and instruction set architectures. AOSP needs a reference target that is flexible, configurable, and affordable – independent of any particular hardware, including those from Google. For years, developers have been building Cuttlefish (available on GitHub as the reference device for AOSP) and GSI targets from source. We continue to make those available for testing and development purposes."_

## What’s left in AOSP 16?
Despite the purge, AOSP still ships several buildable reference devices:

| Device family | Purpose                                                      | Location in tree |
| ------------- | ------------------------------------------------------------ | ---------------- |
| Cuttlefish    | The Android platform emulator and Google’s canonical reference for all hardware work | device/google/cuttlefish |
| Trout         | Cuttlefish‑based emulator tailored for Android Automotive OS | device/google/trout |
| Goldfish      | The classic Android Emulator, used by Android Studio         | device/generic/goldfish |
| DragonBoard 845c / RB5 / HiKey960 | Dev boards supported by Linaro           | device/linaro |
| Khadas VIM3 / VIM3L | Dev boards supported by BayLibre                       | device/amlogic/yukawa |


## Why losing Pixel device configuration hurts
* **More reverse‑engineering, less learning.** Pixel configurations have long served as living documentation of how Google expects a modern Android device to be wired up. Without them, independent developers must diff factory images, sniff partitions and guess which kernel configs or SELinux rules changed.
* **Harder for Custom ROMs.** Developers working on GrapheneOS, LineageOS and others will have to reverse-engineer Pixel support from now on
* **No longer an option for platform developers.** A lot of people have used Pixels as development machines in the past to try out changes to platform code

### Cuttlefish as reference platform
Cuttlefish is the main reference platform from now on, which is fine for most of the code but it becomes more restricted the closer you get to the hardware. Sure, there are emulation layers for most subsystems, and reasonably good support for secure boot, but there is always a point when emulation fails to match reality. Having the Pixel device configurations available was nice because it gave us several examples to work from, each with different characteristics and HALs. Furthermore, the Cuttlefish device configuration has a lot of Cuttlefish specifics which muddy the waters somewhat

### Reading the tea leaves: cost cutting and a narrower funnel
Google hasn't said the move is about money, but AOSP maintenance is undeniably a cost center - it generates no direct revenue. Combined with last quarter's decision to [make aosp‑main read‑only](https://source.android.com/docs/setup/about/faqs#main-merge) and do active development on a private branch, the message is clear: Google wants to spend fewer engineering hours on public infrastructure and more on shipping Android for its own products.

This is not a sign that Android will turn closed‑source. Google explicitly reiterated that _"AOSP is not going away"_, and the Apache 2.0 licence isn't changing. But it is another step back from the "AOSP first" philosophy.

### Where do we go from here? - A call to action
* **Join the community.** This is where [aosp-devs.org](https://aosp-devs.org) can help by sharing knowledge on how device integration works. Join our [Discord server](https://discord.gg/hH59SPKYv8) if you have any questions or just want to share the wisdom on getting your device work.
* **Upstream fixes to generic targets.** Cuttlefish, Trout and Goldfish are still one Gerrit CL away; improvements there benefit everyone.
* **Support community distros and reference boards.** There is a lot going on beyond that offered by Google. There are many Custom ROM projects, including [LineageOS](https://lineageos.org/), [GrapheneOS](https://grapheneos.org/), and [/e/OS](https://e.foundation/e-os/). For embedded Android there are community projects such as [Glodroid](https://glodroid.github.io/) and [Raspberry Vanilla](https://github.com/raspberry-vanilla). Join those efforts or sponsor the work.


Android has always grown through collaboration. Google's retreat makes that collaboration harder, but also more necessary than ever. The future of open Android now depends less on Mountain View and more on _us_.



