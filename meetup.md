---
layout: default
---

# The AOSP and AAOS Meetup

![](/assets/images/aospandaaos-logo.png)

The AOSP and AAOS meetup is an online meeting place for people working with
the open source parts of Android, especially AOSP and Android Automotive.
The goal is to share practical experience: how people build products, solve
technical problems, test and debug systems, and work with the Android platform
in the real world.

Meetings are held every two months. A typical session lasts about one and a
half hour and includes a short welcome, one or two talks, and time for
discussion and networking.

## Joining a meetup

Upcoming meetup details are published on the individual event pages below.
Announcements are made through *aosp-devs.org* and the
[aosp-devs Discord server](https://discord.gg/hH59SPKYv8). You can follow
the site [RSS feed](/feed.xml) as well.

Access details are shared through the channels listed on each event page.

## Upcoming events

<ul>
{% for meetup in site.meetup %}
  <li>
    <a href="{{ meetup.url }}">{{ meetup.title }}</a>
  </li>
{% endfor %}
</ul>

## Past events
[All talks are recorded and are available online](meetups-past.html)


## Speaking at a meetup

Input is welcome from all members of the group. Talks can be formal or
informal: slides, demos, short presentations, or open discussions are all
useful.

Typical topics include:

* good sources of information about AOSP, including conferences, blog posts,
  and other community resources
* running AOSP on real hardware, for example Raspberry Pi
* the Soong build system and Blueprint
* testing and debugging
* emulators such as Cuttlefish, Goldfish, and Trout
* security topics including SELinux, seccomp, and sandboxing
* encryption, secure boot, and trusted execution environments

If you have something to say, get in touch on Discord or by email. See the
contact details on [about](/about/).

## History

The meetup started in March 2022 as an independent online series for AOSP and
AAOS developers by Chris Simmonds. For the first years, it was spread across two places:

* [aospandaaos.github.io](https://aospandaaos.github.io/) for slides, videos,
  and past meetup pages
* [Meetup.com](https://www.meetup.com/the-aosp-and-aaos-meetup/) for event
  listings and RSVPs

The meetup is now continued here on *aosp-devs.org*, which is the main entry
point for new events. Slides and videos from past talks remain available on
the [AOSP and AAOS meetup archive](https://aospandaaos.github.io/meetup.html).
