---
layout: post
excerpt_separator: <!--more-->
title:  "What Recent Android Changes Mean for AOSP and Open Source"
author: Serban Constantinescu, Chris Simmonds
---

There has been a lot of debate about the recent changes in the way that AOSP is developed, and whether that will affect our ability to develop independent, open source versions of Android.

**TL;DR: AOSP remains open source and releases should increase in frequency**
<!--more-->

On 27 March 2025, [Google announced changes to the Android platform development model](https://source.android.com/docs/setup/about/faqs#main-merge). While some interpreted these changes as [Android becoming more closed](https://www.androidauthority.com/google-android-development-aosp-3538503/), the reality is more positive.

The [Android Open Source Project](https://source.android.com/) (AOSP) is one of Google’s most influential open source contributions. It powers an incredibly broad range of devices, from phones and TVs to cars and even coffee machines. In fact, it’s the most widely deployed operating system in the world, used even by companies like [Facebook](https://www.meta.com/en-gb/blog/meta-horizon-os-open-hardware-ecosystem-asus-republic-gamers-lenovo-xbox/) and [Amazon](https://developer.amazon.com/docs/fire-tv/fire-os-overview.html) – organizations outside of Google’s officially approved ecosystem that do not have a licence to use the Google services (e.g. Google Mobile Services for smartphones and tablets, Google Automotive Services for cars, Google TV Services for TVs).

Therefore when Google changes how it develops Android, the implications are significant for everyone involved.


## How AOSP development works at Google
Google’s engineering teams develop the Android operating system for emulators (e.g. Goldfish,  Cuttlefish), Google Pixel devices and a limited number of Android partners that ship certified devices (i.e. licensed to use Google services) across the officially supported form factors [smartphones and tablets](https://www.android.com/), [Android Automotive](https://built-in.google/cars/), [Android TV](https://www.android.com/tv/), [Wear](https://wearos.google.com/), and [Android XR](https://www.android.com/xr/).

These products don’t run AOSP directly. Instead, Google develops internal forks of Android, by form factor, that include proprietary frameworks, APIs, and hardware support. As a result, most of the new Android code is already [developed in private](https://groups.google.com/g/android-platform/c/MDzmcEgxFPw/m/BY-ESnoEqg0J) and the tip of the AOSP main branch is never thoroughly tested by Google’s own teams, leading to [frequent issues](https://issuetracker.google.com/issues?q=status:open%20componentid:381517&s=created_time:desc) for downstream users who tried to build from it.

Still, on a roughly annual basis, Google would snapshot its internal development tree, remove proprietary code, and push out a stable AOSP branch (e.g. [android-12.0.0_r1](https://groups.google.com/g/android-building/c/ChjvrI4jGsU/m/p3tZGLCNAAAJ)). This snapshot brought the majority of new code to the public, but only after it was ready for release.


## What has changed
In simple terms, Google now actively discourages using the AOSP main branch by making it private. Meanwhile, [they’re reinforcing their commitment to releasing stable, open source Android versions](https://source.android.com/docs/setup/about/faqs#:~:text=Our%20single%20most%20important%20goal%20with%20the%20AOSP%20is%20to%20make%20sure%20that%20open%2Dsource%20Android%20software%20is%20implemented%20as%20widely%20and%20compatibly%20as%20possible%2C%20to%20everyone%27s%20benefit.). 

Here’s what this means:
* **The development of the next Android release takes place privately until it’s ready for release**, which is largely [unchanged from before](https://groups.google.com/g/android-platform/c/25aEVdSQ360) - except for the few projects previously developed as AOSP-first (Bionic, Bluetooth, Cuttlefish, Virtualization). It is important to note that in the past, even official Android OEMs struggled to [contribute](https://android-review.googlesource.com/c/platform/frameworks/base/+/2403952) to projects that were not AOSP-first.

* **Android will continue to be published to AOSP via the android-latest-release branch**. After internal development concludes, a stable, thoroughly tested branch is pushed to AOSP. Thanks to the Trunk Stable improvements described below, this will now happen more frequently than in the past.

* **The AOSP contribution process has changed and is likely more opaque**. The [new process](https://source.android.com/docs/setup/about/faqs#contribute) could require more effort from submitters, and mirrors the work previously done within Google when contributions were made to non-AOSP-first projects.

The [Android common kernels](https://source.android.com/docs/core/architecture/kernel/android-common) (ACKs) continue to be developed in the open and upstreamed to [kernel.org](http://kernel.org), while the Android [Native Development Kit](https://developer.android.com/ndk) (NDK) continues to be developed in the open on [GitHub](https://github.com/android/ndk).

While this is disappointing for those who wish all development were public – it has largely already been the norm for Android. Therefore, in essence, very little changes and for most, it will remain business as usual – aside from making it harder to speculate upcoming features through the crumbles of AOSP-first projects.


## How Trunk Stable could actually improve things
Google also recently announced a Trunk Stable development mode, which includes a [new flag-based development model](https://source.android.com/docs/setup/build/feature-flagging) and more [frequent Android releases](https://android-developers.googleblog.com/2024/10/android-sdk-release-update.html) - changes that could positively impact the downstream open source community.

Under this model, features are built behind feature flags and remain dormant until they’re ready to be enabled or included for a specific device or form factor. Internally, this approach lets Google improve quality, by only enabling features when ready, and avoid forking the codebase for each form factor, potentially leading to a more unified codebase across devices.

The new quarterly release schedule for the Android codebase - now including new features rather than just security fixes - offers several potential benefits for downstream projects:

* **Faster access to new features**: Features are no longer bound by the yearly release cycle and can be shipped quarterly if they’re ready.

* **Less fragmentation and fewer bugs**: Features can now be disabled until ready for release, after proper testing, or selectively enabled only for the form factors that need them. This can over time lead to a unified codebase across form factors.


### Impact on other form factors like Android Automotive
For Android Automotive specifically, it should be business as usual. Automotive development has never been fully public, similar to the rest of Android. Google has not indicated that Automotive tags won’t remain public.

Moreover, Trunk Stable might help unify code across all form factors. By using the same core codebase, it could become easier for Google - and in turn, downstream developers - to build on top of a single, more frequently updated version.


### Why we believe Android’s open source future is here to stay
Google significantly benefits from the innovation that arises from keeping Android open – expanding the reach of its core business by delivering its services as widely as possible.

The device ecosystem is an interconnected web of software and [hardware suppliers that work together to deliver devices](https://electronics360.globalspec.com/article/20774/techinsights-teardown-google-pixel-fold#:~:text=Samsung%E2%80%99s%205G%20NR,Murata%E2%80%99s%20saw%20filters). All of these need access to an open source ecosystem so that they can develop their IP, which in return enables Google and its partners to build new devices and form factors.

One prominent example of large-scale innovation is the [Android support for RISC-V](https://opensource.googleblog.com/2023/10/android-and-risc-v-what-you-need-to-know.html). Though now officially embraced by Google, it was originally initiated by [Alibaba](https://riscv.org/blog/2021/11/how-alibaba-is-porting-risc-v-to-the-android-os-guoyin-chen-alibaba/) and wouldn't have been possible without AOSP being open source.


## Conclusion
While the recent changes to the Android development model may feel unsettling to those who want fully transparent development, the impact on the broader Android ecosystem is minimal and does not practically change things too much.
