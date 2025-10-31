---
layout: default
---

# aosp-devs.org October newsletter

Welcome to the tenth aosp-devs newsletter, keeping you up to date with things
happening in the AOSP developer community.

Since the newsletter is not on-time (again), it misses halloweeeeeeen.


## News update about the Application Sideloading Changes

After the first blog post from F-Droid
[Let's talk security: Answering your top questions about Android developer verification](https://android-developers.googleblog.com/2025/09/lets-talk-security-answering-your-top.html?m=1),
they have published a second
post [What We Talk About When We Talk About Sideloading](https://f-droid.org/en/2025/10/28/sideloading.html)
now. It also contains a reference to the new website:
[Keep Android Open](https://keepandroidopen.org/)

Here is the last public statement from Google from September:
[Let's talk security: Answering your top questions about Android developer verification](https://android-developers.googleblog.com/2025/09/lets-talk-security-answering-your-top.html?m=1)


## LPC Schedule is out

The [schedule](https://lpc.events/event/19/timetable/?view=lpc) for the Linux
Plumbers Conference this year is out. It continues to feature the
[Android MC (Micro Conference)](https://lpc.events/event/19/contributions/1992/),
but also contains Android related talks in other tracks.


## Talk Recordings

[droidcon Berlin](https://berlin.droidcon.com/) and the
[AOSP devroom at IndiaFOSS](https://fossunited.org/indiafoss/2025/devrooms/aosp)
were already featured in the last newsletter, but now all talk recordings are
out.

All AOSP devroom talks

* Strengthening the AOSP Developer Community: Tools, Boards & Collaboration - Sumit Semwal
* First Step into Open Source with AOSP - Kavibhagya K
* AOSP Testing at scale using CuttleFish in the Cloud - Vishal Bhoj
* Implementing a Custom HAL in AOSP - Rutvij Trivedi
* AOSP E2E: Internals, Security, Optimization - Building ROM & Automotive - Immanuel Raj
* Libcamera: Is it next universal AOSP Camera HAL? - Jaimin Parmar
* Android doesn’t impact general purpose embedded solutions any more ! - Does it ? - Khasim Syed Mohammed
* AOSP without the Baggage: Booting with vanilla Linux Kernel - Amit Pundir

are on the Youtube playlist
[AOSP Devroom at IndiaFOSS 2025](https://www.youtube.com/watch?v=WOn_fqGwKyk&list=PLOGilj110olwA2QSne1jYdWTPJY6OLR1T&index=1).

And a selected list of AOSP/AAOS-related talks from droidcon berlin is:

* [Open source and Android Automotive OS - Chris Simmonds - droidcon Berlin 2025](https://www.youtube.com/watch?v=H7fx3pnaHp4)
* [AIDL HAL by Example: Using Hardware from Android Application - Viktor Mukha - droidcon Berlin 2025 ](https://www.youtube.com/watch?v=JnlXA9XVe3g)
* [It's time to develop apps for Android cars - Chris, Sabine and Gabriel - droidcon Berlin 2025 ](https://www.youtube.com/watch?v=q5L8qWoG3dw)
* [Inside Android: Context, Binder IPC, Zygote - Ioannis Anifantakis - droidcon Berlin 2025](https://www.youtube.com/watch?v=AXUu-_fEyD0)


## Android Building Google group

The newsletter highlights a thread on the
[Android Building Google group](https://groups.google.com/g/android-building):
[AOSP build being so resource demanding is frustrating - can we optimize?](https://groups.google.com/g/android-building/c/SE4cjLQoc9E)

It contains a lot of good responses and material. One quote:

> 16GiB wasn't enough to build comfortably a decade ago. and while, yes,
> if you were their boss you could have an engineer try to reduce those
> requirements ... but you'd have a hard time justifying to _your_ boss
> why that engineer wasn't fixing something that would improve the
> product. especially because the cost of 128GiB of ram isn't going to
> pay that engineer's wages (even if they're on minimum wage!) for one
> whole 40 hour week.
>
> https://en.wikipedia.org/wiki/Opportunity_cost

And it also features more information about the technical details of the
Android build system. Have a look!


## And other notes from Discord

Since in October there were a lot of good discussions on Discord, the following
list is only a short excerpt. Feel free to join the [Discord server](https://discord.gg/hH59SPKYv8)
and listen directly.

Example HAL implementation: [aosp.local-manifests.paradoxcat-infineon-radar](https://github.com/Paradox-Cat-GmbH/aosp.local-manifests.paradoxcat-infineon-radar) and [RadarDemoApp](https://github.com/Paradox-Cat-GmbH/RadarDemoApp):
[Discussion on Discord](https://discord.com/channels/1294292505419841678/1294292505927487510/1430132070751141999)

Another Example HAL implementation: [Custom-HAL-Demo-LED](https://github.com/Silicon-Signals/Custom-HAL-Demo-LED),
[Discussion on Discord](https://discord.com/channels/1294292505419841678/1346847709520203908/1420438203126644806)

Talk: [Transitioning to memory safety: lessons from the Android project - Jeffrey Vander Stoep](https://www.youtube.com/watch?v=2Pm8l5O26ds)

Discussion about the ongoing (Linux kernel) mainline efforts by LineageOS and the currently
stalled project [AOSP Mainline](https://github.com/AOSPM):
[Discussion on Discord](https://discord.com/channels/1294292505419841678/1294292505927487510/1427825005592445009)

LineageOS has a good summary
[Changelog 30 - Sleek Sixteen, Streamlined Suite, Future Flow](https://lineageos.org/Changelog-30/)
of the recent release strategy changes by Google: Security releases only every
four months, and QPR delayed/not-released.

Interesting talk about multiple displays and foldables:
[Discussion on Discord](https://discord.com/channels/1294292505419841678/1294292505927487510/1432143595187605576)

Talk about integrating a Renesas camera into a Qualcomm-based board:
[Discussion on Discord](https://discord.com/channels/1294292505419841678/1309452712852721696/1433358326648799275)

Talk about OP-TEE and building:
[Discussion on Discord](https://discord.com/channels/1294292505419841678/1346847709520203908/1424853141505052896)


## Upcoming Events

### AOSP and AAOS November Meetup (online)

* Link: [The AOSP and AAOS November Meetup](https://www.meetup.com/the-aosp-and-aaos-meetup/events/311085579/)
* Date and time: Wednesday, Nov 19 · 8:00 PM to 10:00 PM CET
* Location: online with Jitsi Meet


### Linux Plumbers Conference - Android Micro Conference (in-person and remote)

* Link: [Android MC](https://lpc.events/event/19/contributions/1992/)
* Date: Dec 11 – 13, 2025
* Location: Toranomon Hills Forum, Tokyo, Japan
* Schedule: [LPC detailed schedule](https://lpc.events/event/19/timetable/?view=lpc)
