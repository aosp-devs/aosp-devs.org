---
layout: default
---

# aosp-devs.org February Newsletter

Welcome to the second aosp-devs newsletter, keeping you up to date with things happening in the AOSP developer community.

Perhaps the most important thing to mention is that we held our first AOSP devroom at FOSDEM. We believe it was a great success! The recordings are now available on our new YouTube channel: [@aosp-devs](https://www.youtube.com/@aosp-devs). Enjoy watching!


## New Blogposts and Media

[Implementing Custom Hardware Abstraction Layer (HAL) in Android with AIDL](https://siliconsignals.io/blog/implementing-custom-hardware-abstraction-layer-hal-in-android-with-aidl-silicon-signals/)

[About designing a HAL and using it on a Service - by Mairon Lucas Slusarz - ProFUSION Engineering - Feb, 2025 - Medium](https://medium.com/profusion-engineering/about-designing-a-hal-and-using-it-on-a-service-e73861a62ebd)

[Video: HALs in Android 15: AIDL, Apex and the disappearance of VNDK](https://www.youtube.com/watch?v=7lAzdjUQFUg) (See also below) 


## Notes from Discord

Linux kernel driver development and example: “Now this is what I was looking for. A self contained example, instead of the pixel's inheriting four levels of common-ish trees. This I can work with. Many thanks.”:
[Discussion on Discord](https://discord.com/channels/1294292505419841678/1309451559263928340/1335906168689786901)
and [driver example](https://gitlab.baylibre.com/baylibre/amlogic/atv/aosp/kernel/yukawa-device)

Mention of Driver Development Kit (DDK):
[Driver Development Kit (DDK)](https://android.googlesource.com/kernel/build/+/refs/heads/main/kleaf/docs/ddk/main.md?pli=1)

“We use enforce-product-packages-exist() to make sure that we don't have any unknown packages in our build”:
[index : android/device-ti-am62x](https://git.ti.com/cgit/android/device-ti-am62x/commit/?h=d-android15-release&id=62de65160d9324fa0978ac25c3a4f2ae90b9864e)
and
[Discussion on Discord](https://discord.com/channels/1294292505419841678/1294292505927487510/1336265202341253161)

Discussion on “how to best don’t fork the aosp”:
[Discussion on Discord](https://discord.com/channels/1294292505419841678/1294292505927487510/1336022352261156895)

Discussion about upstream camera HALs:
[Discussion on Discord](https://discord.com/channels/1294292505419841678/1294292505927487510/1341318937945833502)

Discussion about kernel module development and BOARD\_DO\_NOT\_STRIP\_VENDOR\_MODULES
[Discussion on Discord](https://discord.com/channels/1294292505419841678/1309451559263928340/1342687078403674203)
and
[cs.android.com](https://cs.android.com/android/platform/superproject/main/+/main:device/google/gs101/BoardConfig-common.mk;l=350?q=BOARD_DO_NOT_STRIP_VENDOR_MODULES)

Discussion about using apex for HALs: [Discussion on Discord](https://discord.com/channels/1294292505419841678/1294292505927487510/1343400768589398070)
and
[source.android.com - Make apex smaller](https://source.android.com/docs/core/ota/vendor-apex#make_apex_smaller)

Discussion about persistent, e.g. the persistent flag in the Android Manifest:
[Discussion on Discord](https://discord.com/channels/1294292505419841678/1294292505927487510/1344294282215030867)
[developer.android.com - application-element - persistent](https://developer.android.com/guide/topics/manifest/application-element#persistent)

"Hi all! I am looking to get some feedback from Android developers (and beyond)
on current European regulations impacting Android security. Please fill out
this form if you are interested in connecting!":
[Discussion on Discord](https://discord.com/channels/1294292505419841678/1294292505927487510/1338450246467981332)

Post about internal and external, e.g. to track down changes from AOSP to internal resources at Google:
[Discussion on Discord](https://discord.com/channels/1294292505419841678/1294292505927487510/1339270629966479482)

"AOSP-first" projects:
[Discussion on Discord](https://discord.com/channels/1294292505419841678/1294292505927487510/1339273701178478623)


## Upcoming Events

### Embedded Recipes (in-person)

*   Link: [https://embedded-recipes.org/2025/](https://embedded-recipes.org/2025/)
*   Date: May 14-16th 2025
*   Location: Nice, France


### Linaro Connect (in-person)

*   Link: [https://www.linaro.org/connect/](https://www.linaro.org/connect/)
*   Date: Wednesday 14 May - Friday 16 May 2025
*   Location: Lisbon, Portugal


### AOSP and AAOS March Meetup (online)

*   Link: [The AOSP and AAOS March Meetup](https://www.meetup.com/the-aosp-and-aaos-meetup/events/305840348/)
*   Date and time: Wednesday, March 19, 2025, 7:00 PM to 9:00 PM CET
*   Location: online/zoom
*   Schedule:
    *   18:15 Talk 1: Using Vendor APEX in AOSP
    *   18:45 Talk 2: What to expect in Android 16
    *   19:15 "What are you working on?"
        

## Past events

### FOSDEM  and AOSP devroom (in-person)

*   Link: [https://fosdem.org/2025/](https://fosdem.org/2025/)
*   Link to devroom: [https://fosdem.org/2025/schedule/track/aosp/](https://fosdem.org/2025/schedule/track/aosp/)
*   Recordings are online: On the FOSDEM webpage and on youtube. Direct link to the playlist: [FOSDEM 2025 - AOSP devroom](https://www.youtube.com/playlist?list=PLwfiJmU4qhXsXi6-HoUvs3zdORvE55Y-M) 
    

### opersys: HALs in Android 15: AIDL, Apex and the disappearance of VNDK (online)

*   Link to recording: [https://www.youtube.com/watch?v=7lAzdjUQFUg](https://www.youtube.com/watch?v=7lAzdjUQFUg)
*   Date: 2025-02-19

