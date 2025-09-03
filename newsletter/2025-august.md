---
layout: default
---

# aosp-devs.org August newsletter

Welcome to the eighth aosp-devs newsletter, keeping you up to date with things
happening in the AOSP developer community.

And … again three days too late. Who would have thought that?


## Upcoming changes by Google for Application sideloading

In August Google posted a change to the possibility of sideloading Apps on
compatible Android devices. See
[A new layer of security for certified Android devices](https://android-developers.googleblog.com/2025/08/elevating-android-security.html).

The main message: Sideloading aka third party App Story are still possible. But
also the sideloaded apps are checked by Google now and Developers need to
create an account to sign their Apps for sideloading.

The timeline is

>  Here is the timeline to help you plan:
>
> * October 2025: Early access begins. Invitations will be sent out gradually.,
> * March 2026: Verification opens for all developers.,
> * September 2026: These requirements go into effect in Brazil, Indonesia, Singapore, and Thailand. At this point, any app installed on a certified Android device in these regions must be registered by a verified developer.,
> * 2027 and beyond: We will continue to roll out these requirements globally.

And here is the [discussion on discord](https://discord.com/channels/1294292505419841678/1294292505927487510/1412024397916672092).

This new security model is only enforced on Android-compliant devices. If you
build your own AOSP and ship without
[Google Mobile Services](https://en.wikipedia.org/wiki/Google_Mobile_Services)
you are not affected.


## Some of the talk recordings of the AAOS Bootcamp have been released

Previously there were only some small signs that Google is running a bootcamp
with presentation for thier automotive partners. E.g. some dropped PDF files (and
really valuable slides) on
[source.android.com: Car framework core](https://source.android.com/docs/automotive/car-framework-core).

But now Denis Nekliudov from Google posted on
[LinkedIn](https://www.linkedin.com/posts/nekdenis_if-you-ever-wondered-what-is-the-android-activity-7361247882152153088-dHdn/)
some recordings of the bootcamp. They are available on this
[youtube playlist](https://www.youtube.com/playlist?list=PLWz5rJ2EKKc9meeN35UTsUJpbt7nZWXHf).

As we learned these talks were held on a third day of the bootcamp and intended
to be 101 beginner sessions. The slides were already a good resource for AAOS
topics, but the recordings are super exciting.

Here is also the [discussion on Discord](https://discord.com/channels/1294292505419841678/1309452712852721696/1405201266077995129).


## Notes from Discord

[Some turbulence at CalyxOS](https://lwn.net/Articles/1033042/)

Boot time optimization, Tips, tricks and notes, e.g. Baseline profiles and boot time profiles:
[Discussion on Discord](https://discord.com/channels/1294292505419841678/1309452712852721696/1405082820333801482)

Chris Simmonds on [Using Yocto to build AOSP](https://www.linkedin.com/pulse/using-yocto-build-aosp-chris-simmonds-ymhof/)

Discussion on property implementation the VHAL, and callbacks:
[Discussion on Discord](https://discord.com/channels/1294292505419841678/1294292505927487510/1407621420879450112)

Google has dropped support for Pixel devices in the AOSP. Already covered in
the previous newsletter, but still something to discuss:
[Discussion on Discord](https://discord.com/channels/1294292505419841678/1294292505927487510/1408413595783528631)

Question about international shipping of [Jonathan Levin books on Android](https://newandroidbook.com/)
[Discussion on Discord](https://discord.com/channels/1294292505419841678/1294292505927487510/1408866621384294431)


## Upcoming Events

### AOSP and AAOS September Meetup (online)

* Link: [The AOSP and AAOS September Meetup](https://www.meetup.com/the-aosp-and-aaos-meetup/events/309610342/)
* Date and time: Wednesday, September 17, 2025, 7:00 PM to 9:00 PM CEST
* Location: online with Jitsi Meet


### Android Open Source Project (AOSP) devroom at IndiaFOSS 2025 (in-person)

* Link: [IndiaFOSS](https://platform.fossunited.org/indiafoss/2025)
* Link to the devroom and CfP: [Android Open Source Project (AOSP) devroom](https://fossunited.org/indiafoss/2025/devrooms/aosp)
* CfP: Closed
* Date and time: 19 - 21 September 2025
* Location: NIMHANS Convention Centre, Bengaluru, India


### DroidCon Berlin (in-person)

* Link: [droidconberlin](https://berlin.droidcon.com/)
* Date: September, 24th – 26th
* Location: Berlin, Germany
* Call for Papers: Closed


### Linux Plumbers Conference - Android Micro Conference (in-person and remote)

* Link: [Android MC](https://lpc.events/event/19/contributions/1992/)
* Date: Dec 11 – 13, 2025
* Location: Toranomon Hills Forum, Tokyo, Japan
* Call for Papers: open


## Past Events

### Open Source Summit Europe / Embedded Linux Conference Europe (in-person)

* Link: [Open Source Summit Europe](https://events.linuxfoundation.org/open-source-summit-europe/about/about-oss/)
* Link: [Embedded Linux Conference](https://embeddedlinuxconference.com/)
* No recordings yet
* Date: 25-27 August 2025
* Location: Amsterdam, Netherlands


### AOSP Session @ Open Source Summit India (in-person)

* Link: [Open Source Summit India](https://events.linuxfoundation.org/open-source-summit-india/)
* Link and Recording: [Bootloops & Coffee: The Daily Grind of an AOSP Developer - Sumit Semwal & Amit Pundir, Linaro Ltd.](https://ossindia2025.sched.com/event/23Jkt/bootloops-coffee-the-daily-grind-of-an-aosp-developer-sumit-semwal-amit-pundir-linaro-ltd?iframe=no)
* Date:  Tuesday August 5, 2025 3:05pm - 3:30pm IST
* Location: Hyderabad, India
