---
layout: default
---

# Past Events

## The July 2026 Meetup

15<sup>th</sup> July 2026

### Introduction
The announcement that the AOSP and AAOS Meetup is migrating from Meetup.com
to aosp-devs.org

[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2026-july-introduction.pdf)

### Talk 1: The OEM VHAL

The default Vehicle HAL that is part of AAOS has strict rules about which
vehicle signals are available to apps. For system apps signed by the OEM, all
signals are available. For all other apps, only a very restricted subset is
allowed.

The OEM VHAL extends the vehicle property interface to allow all apps
controlled access to all signals, mediated at run-time by the extended VHAL.
The OEM VHAL is a work in progress, and feedback is welcome.

Jan Kubovy (BMW)

[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2026-july-jkubovy-oem-vhal.pdf)
[video](https://peertube.tech/w/i3V53FYHrWRWBZHMgBBv7u)


## The May 2026 Meetup

27<sup>th</sup> May 2026

### Talk 1: Cuttlefish Development & Deployment

Cuttlefish is an Android based VM that can be used for Android Platform
development, kernel development, and app development amongst other things.
We'll discuss how to set one up, launch locally for development, remotely for
your CI usecases, and configure these environments as needed.

Sergio Rodriguez, Google

[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2026-may-srodriguez-cuttlefish.pdf)
[video](https://peertube.tech/w/shUbZtWqcMHY8cCYyMPDps)


## The March 2026 Meetup

18<sup>th</sup> March 2026

### Talk 1: Acceleration x AOSP: Slashing build times without migration

AOSP development often involves long wait times and "variant explosion" across
different hardware targets. This talk shows how to use process-level caching
and distributed execution to cut two-hour builds down to twenty minutes without
needing to touch your Soong or Ninja scripts.

Peleg Rand, Incredibuild

[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2026-march-prand-incredibuild.pdf)
[video](https://peertube.tech/w/oe68nnFm3PcxTruYy8ufza)


### Discussion: the state of Embedded Android

A round table discussion about Embedded Android: i.e. Android built into
devices that are beyond the profiles that Google support (Phones, Tablets, TVs,
Wearables, Automotive)

[video](https://peertube.tech/w/76uRDdi7QSDEjPuSf8tgus)


## The January 2026 Meetup

28<sup>th</sup> January 2026

### Introduction
[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2026-january-introduction.pdf)

### Talk 1: Keeping Android up to date when the OEM fails to

The Advantech TPC-107W only supports Android 10 without secure boot. This talk
shows how running the latest software was achieved without any help from
Advantech and which challenges had to be overcome. It also briefly goes into
why this was done and why you might want to do the same

Michael Zimmermann, 7/LAB

[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2026-january-mzimmermann-keeping-android-up-to-date.pdf)
[video](https://youtu.be/fdC-_l0dxtg)

### Talk 2: Debugging Android OS at Scale: AI-Powered Log Analysis

AOSP builders spend hours manually correlating events across logcat, dmesg, and
bugreports to debug system issues. logcat.ai uses AI to automate this,
performing multi-step root cause investigations through autonomous "deep
research" that follows leads step-by-step. We're making enterprise-grade
debugging accessible to individual developers and open-source projects through
our OSS program at logcat.ai/oss

Varun Chitre, logcat.ai

[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2026-january-vchitre-logcatai.pdf)
[video](https://youtu.be/yDpInpfV85g)

## The September 2025 Meetup

17<sup>th</sup> September 2025

### Talk 1: Mastering SELinux in AOSP: From Frustration to Control

SELinux is often seen as a blocker when working with AOSP — especially when "avc: denied" messages get in the way. But when understood and managed properly, SEPolicy becomes a powerful tool to harden and structure your system. In this talk, you’ll learn:
* Why SELinux is critical to Android security
* How to manage and maintain SEPolicy in real AOSP projects
* Proven techniques to debug and fix policy issues

Daniel Fages

[video](https://youtu.be/SykYnPC5Yrg)


## The July 2025 Meetup

16<sup>th</sup> July 2025

### Talk 1: Writing Android system apps

Normal apps are limited by the constraints of their sandbox. System apps, on the other hand,
can escape the sandbox to varying extents. In this talk, I explain the various levels of
system app and how to build them in AOSP

Chris Simmonds

[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2025-july-system-apps.pdf)


## The March 2025 Meetup

19<sup>th</sup> March 2025

### Talk 1: Using Vendor APEX in AOSP

Vendor APEX modules allow developers to package entire feature implementations, such as the WiFi HAL, into a single, self-contained unit. The advantages are faster iteration, simplified testing, easier debugging, and modular updates.

Renjith Rajagopal 

[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2025-march-rrajagopal-vendor-apex.pdf)
[video](https://youtu.be/6aS67PqueCw)


### Talk 2: What to expect in Android 16
Android 16 is early this year, in Q2 in fact. Apart from the release schedule, what else is new? Here is a summary of the things that we can expect.

Mishaal Rahman

[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2025-march-mrahman-android-16.pdf)
[video](https://youtu.be/kJTu60Lu9Rw)


## The January 2025 Meetup

29<sup>th</sup> January 2025
### Talk 1: Bugreport is your friend

Using the bugreport command a lot of issues ranging from audio mixing, screen flicker, and issues regarding Car power policies can be resolved effectively. In this talk I would like to highlight the information from the bugreport that could help resolve various issues

Ramalinga Prasad Tadapalli

[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2025-january-prasad-bugreport.pdf)
[video](https://youtu.be/Myx5fgggYto)

### Talk 2: Exploring Android Kiosk Variants

Defining requirements for restricted Android UI

Igor Kalkov-Streitz, Emteria

[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2025-january-iks-kiosk.pdf)
[video](https://youtu.be/3UzLowj-3xQ)


## The November 2024 Meetup

20<sup>th</sup> November 2024

### Talk 1: The AOSP community and aosp-devs.org
We launched aosp-devs.org at the start of November. Here, Chris Simmonds talks
about the genesis of the group, its aims and achievements so far

Chris Simmonds

[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2024-november-csimmonds-aosp-devs.pdf)
[video](https://youtu.be/YE7G_cwkAR8)


## The September 2024 Meetup

25<sup>th</sup> September 2024

### Talk 1: The COVESA AOSP SDK

Through the Automotive AOSP App Framework Standardization Expert Group, members
of COVESA are working on an SDK that provides a set of libraries which allow
third-party applications to access some automotive features in a way that is
independent of manufacturer and model

Daniele Bonaldo, Snapp Automotive

[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2024-september-dbonaldo-covesa-sdk.pdf)
[video](https://youtu.be/Hlixp4lOOQY)

### Talk 2: Feedback from OSS and Linux Plumbers Conference in Vienna
Last week there were two important conferences: the Open Source Summit Europe (OSSE)
and Linux Plumbers Conference (LPC), both taking place in the city of Vienna.
There were a lot of AOSP developers there and many talks on AOSP topics. Here,
I will give an overview of the topics presented and give you a flavor of some
of the conversations that went on in the hallways in between

Chris Simmonds, 2net

[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2024-september-csimmonds-notes-from-vienna.pdf)
[video](https://youtu.be/9UuQO6vVkv0)



## The July 2024 Meetup

17<sup>th</sup> July 2024

### Introduction
[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2024-july-introduction.pdf)

### Talk 1: AOSP Development Environment best practices, tips, and tricks

Let us talk about tools we use for AOSP development. In this presentation we will focus on using Visual Studio Code and do some live demos

Roman Illarionov and Viktor Mukha, Paradoxcat

[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2024-july-vmukha-tips-and-tricks.pdf)
[video](https://youtu.be/vuy4We_mbJg)

### Talk 2: AAOS on Raspberry Pi: an on-going project

An update on where we are with this project

Chris Simmonds

[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2024-july-csimmonds-a3m-rpi.pdf)
[video](https://youtu.be/Q0BYKAb1BHw)


## The May 2024 Meetup

22<sup>nd</sup> May 2024

### Introduction
[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2024-may-introduction.pdf)
[video](https://youtu.be/Z-REBePidqA)

### Talk 1: Introducing AOSP Meetup Projects
Chris Simmonds

[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2024-may-projects.pdf)
[video](https://youtu.be/QXuIqwiiRFY)


### Talk 2: Automotive AOSP Ecosystem: challenges and opportunities for App Developers

In the last few years we've seen an increasing adoption from Automotive OEMs of
Android based In-Vehicle Infotainment (IVI) platforms. While there are
differences between platforms running with and without Google Automotive
Services (GAS), the majority of apps can actually be built once and run
anywhere, which is a paradigm shift for the industry. We'll discuss the
different categories of automotive apps and what is being done at COVESA to
avoid ecosystem fragmentation.

José Freitas, Faurecia Aptoide 

[video](https://youtu.be/zeH9LC2XHWs)

### Talk 3: You Can't Escape the Past: How early design decisions continue to influence Android today
Chet Haase talks about the team that built the Android operating system and why
they chose to do certain things certain ways: the graphics stack, security
model, the app programming language ... these are things that affect us every
day

Chet Haase

[video](https://youtu.be/ZDnlKg5Y7TA)


## The March 2024 Meetup

20<sup>th</sup> March 2024

### Introduction
[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2024-march-introduction.pdf)


### Talk 1: Android Fragmentation in the Automotive Industry

Android fragmentation is becoming a real issue in the automotive industry.
What is it and what can we do to prevent it?

Juhani Lehtimäki, Snapp Automotive

[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2024-march-jlehtimaeki-fragmentation-in-aaos.pdf)
[video](https://youtu.be/ZC2MELSKf98)


### Talk 2: What to expect in Android 15

While the source code for this year's Android 15 'Vanilla Ice Cream' release
won't be made public before early September (estimated), there's a lot we can
glean about this release from Google's current developer previews, AOSP code
changes, and documentation. Here's a summary of what to expect

Mishaal Rahman

[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2024-march-mrahman-what-to-expect-in-android-15.pdf)
[video](https://youtu.be/9gZOPiuy8zQ)


## The January 2024 Meetup
24<sup>th</sup> January 2024

### Talk 1: SELinux in Android
How it works and how it's used to make Android more secure

Alan Stokes, Google

[slides](https://docs.google.com/presentation/d/1q-qqTSccLZNteyjgxMRWO971b_UbAKfPPyDHS59O5B4/edit)
[video](https://youtu.be/uI9nk1VDCpY)


### Talk 2: aminilog – AOSP styled logging macros for NDK projects
Stefan Lengfeld, inovex

[video](https://youtu.be/EZbpJKLEmUE) [github](https://github.com/lengfeld/aminilog)


## The November 2023 Meetup
15 <sup>th</sup>November 2023

### Introduction
[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2023-november-introduction.pdf)
[video](https://youtu.be/4CGs93MoDdA)

### Talk 1: Working with custom Android devices
In this session you will learn the most important parts of working on custom
devices. We will cover things like developers boards, board support packages,
AOSP builds, firmware updates, and much more

Erik Hellman

[slides](https://speakerdeck.com/erikhellman/working-with-custom-android-devices-and-aosp-build-system) [video](https://youtu.be/Yds-lc1TD3g)

### Talk 2: Adventures with Systrace - measure and investigate the glass to glass latency in Android
What is the glass to glass latency in Android? This means how much delay is
between the camera, taking a picture, and the screen, to display the picture
again. This presentation is a technical tour through the Android graphics
system and hardware. From the measurement setup, based on cables, LEDs,
photodiodes and an oscilloscope, to camera sensors and the rolling shutter
effect, to displays and refresh rates, to surfaceflinger and vsyncs, and last
but not least to the ultimate tool to debug most of your performance issues, to
Android's systrace

Stefan Lengfeld, inovex

[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2023-november-slengfeld-glass-to-glass-latency.pdf) [video](https://youtu.be/NKP4JcVegbY)

### Q & A
Following the two talks at the meetup there was a Q & A session that covered
topics from the talks and also other (related) topics

[video](https://youtu.be/I2vQmhDSLtw)


## The September 2023 Meetup
27<sup>th</sup> September 2023

### Introduction
<https://2net.co.uk/slides/aosp-aaos-meetup/2023-september-introduction.pdf>

### Talk 1: Interactive AOSP-based cloud streaming solution
Running an AOSP 13 adaptation on an ARM64 cloud server, streaming it to an actual phone at high frame rate and low-latency for touch events.
Simonas Leleiva, iond.io
[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2023-september-sleleiva-aosp-in-the-cloud.pdf)



## The July 2023 Meetup

12<sup>th</sup> July 2023

### Introduction
<https://2net.co.uk/slides/aosp-aaos-meetup/2023-july-introduction.pdf>

### Talk 1: Binder RPC - AIDL for distributed systems
David Brazdil, Google
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2023-july-dbrazdil-rpc-binder.pdf)
[Video](https://youtu.be/undYyHZtiuk)

### Talk 2: Debugging AOSP using Android Studio - revisited
Chris Simmonds, 2net
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2023-july-csimmonds-debug2.pdf)
[Video](https://youtu.be/hy40algJYuY)

### Useful links
* what-changed - list changes in repos between two tags: <https://github.com/aospandaaos/useful-scripts>
* Repoload - a change request download tool: <https://github.com/lengfeld/repoload/>
* A JDB/GDB plugin for VIM: <https://github.com/brookhong/jdb.vim>


## The May 2023 Meetup

24<sup>th</sup> May 2023

### Introduction
<https://2net.co.uk/slides/aosp-aaos-meetup/2023-may-instroduction.pdf>

### Talk 1: Broadcast Radio in AAOS
Simon Osim, Conjure
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2023-may-sosim-broadcast-radio.pdf)
[Video](https://youtu.be/xUMLpF-kM0s)

### Talk 2: RAMSES – An open source 3D graphics tool chain for Android
Klaus Gaßner, Paradox Cat
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2023-may-paradoxcat-ramses.pdf)
[Video](https://youtu.be/1Sa6Tx2-EPM)

### Talk 3: Evolution of an Android OTA management application
Diego Rondini, Kynetics
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2023-may-drondini-ota.pdf)
[Video](https://youtu.be/qdXZhMIWZ8U)


## The March 2023 Meetup

29<sup>th</sup> March 2023

### Talk 1: Devboard maintenance in AOSP
Amit Pundir, Linaro
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2023-march-apundir-devboards-in-aosp.pdf)
[Video](https://youtu.be/VDYhz69xXwc)


### Talk 2: Debugging Made Easy: Tips and Tricks for Android Developers
Chris Hayes, Memfault
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2023-march-chayes-debugging-tips.pdf)
[Video](https://youtu.be/9HcFtcd_DKQ)


## The January 2023 Meetup

11<sup>th</sup> January 2023

### Talk 1: App developers and Android Automotive OS
Al Sutton - Snapp Automotive
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2023-january-asutton-apps-for-aaos.pdf)
[Video](https://youtu.be/IaLsLflXBsc)

### Talk 2: Thoughts about AOSP on Raspberry Pi 4
Chris Simmonds - 2net
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2023-january-csimmonds-rpi4.pdf)
[Video]( https://youtu.be/WAsCXnLOD-A)


## The November 2022 meetup

16<sup>th</sup> November 2022


### Talk 1: ConnectivityService and networking in Android
Diogo Júnior - Critical TechWorks
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2022-november-ConnectivityOnAndroid-DiogoJunior.pdf)
[Video](https://youtu.be/F_lRRKpUuuo)


### Talk 2: Securing iMX6 Android Devices, Part 2
Andrea Scian - DAVE Embedded Systems
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2022-november-Securing_iMX6_Android_Devices-part-2.pdf)
[Video](https://youtu.be/LaSA0xGP81Q)


### Talk 3: Debugging SEPolicy
Chris Simmonds - 2net
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2022-november-csimmonds-selinux.pdf)
[Video]( https://youtu.be/yxhDD3qJyVo)



## The September 2022 meetup

28<sup>th</sup> September 2022

### Talk 1: Notes from Linux Plumbers Conference
Chris Simmonds - 2net
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2022-september-csimmonds-notes-from-lpc.pdf)
[Video](https://youtu.be/hd0qgC16G1w)

### Talk 2: Swimming towards a Software Defined Architecture with Android Trout
Isaac Trefz - OpenSynergy
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2022-september-opensynergy-trout.pdf)
[Video](https://youtu.be/zF_MgP7h_OM)

### Talk 3: You can do better than bug reports
Devon Yablonski - Memfault
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2022-september-memfault-logging.pdf)
[Video](https://youtu.be/QZTqAID3EkU )

### Talk 4: gdb & lldb debugging custom RPI4 linux kernel
Jürgen Weißer
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2022-september-jweisser-rpi4-debug.pdf)
[Video](https://youtu.be/XwQNfCkeumI)
[Files](https://github.com/aospandaaos/gdb_lldb_debugging_custom_RPI4_linux_kernel)


## The July 2022 meetup

20<sup>th</sup> July 2022

### Talk 1: Extending the Vehicle HAL with vendor properties
Chris Simmonds - 2net
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2022-july-hidl-extensions.pdf)

### Talk 2: Debugging native platform code using LLDB
Chris Simmonds - 2net
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2022-july-native-debug.pdf)
[Video](https://www.youtube.com/watch?v=HcuCD7nXeaI)

### Talk 3: Keeping Embedded Android Up To Date
Igor Kalkov-Streitz - Emteria
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2022-july-Emteria-OTA.pdf)
[Video](https://youtu.be/b0oW4Vmmdgw)


## The May 2022 meetup

18<sup>th</sup> May 2022

### Talk 1: Securing iMX6 Android Devices
Andrea Scian - DAVE Embedded Systems  
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2022-may-AOSP_Meetup_Securing_iMX6_Android_Devices.pdf)
[Video](https://youtu.be/cc69ybvH-bM)

### Talk 2: Long term support for Enterprise Android Devices
Rupesh Gujare - NotioNext
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2022-may-android_edla_long_term_support.pdf)

### Talk 3: Introduction to COVESA and the Android Automotive Special Interest Group
Paul Boyes - COVESA
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2022-may-COVESA_Briefing_AOSP_Meetup.pdf)

### Talk 4: Browsing and debugging framework code using Android Studio
Chris Simmonds - 2net
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2022-may-debug.pdf)
[Video](https://youtu.be/SEgBapOKI2g)


## The March 2022 meetup

16<sup>th</sup> March 2022

This was the first meetup of our group. A total of 25 members attended, and I would like to say thanks to everyone who was there, and I hope you are motivated to come along to the next one in May

### Talk 1: Aims and Objectives of the AOSP and AAOS Meetup
Chris Simmonds - 2net
[Slides](https://2net.co.uk/slides/aosp-aaos-meetup/2022-march-introduction.pdf)

### Talk 2: The Cuttlefish Emulator
Chris Simmonds - 2net
[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2022-march-cuttlefish.pdf)

### Talk 3: VHAL SocketComm
Chris Simmonds - 2net
[slides](https://2net.co.uk/slides/aosp-aaos-meetup/2022-march-vhal-socketcomm.pdf)


