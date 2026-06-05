---
layout: default
---

# The AOSP and AAOS Meetup

![](/assets/images/aospandaaos-logo.png)

The AOSP and AAOS Meetup Group is a forum for talking about building,
developing, and testing products based on AOSP (Android Open Source Project)
and AAOS (Android Automotive OS).

Meetups are the main reason for the existence of the group. Meetings are
held every two months starting in January (so, January, March, May, July,
September, and November). The first was in March 2022. Each meeting is about 2
hours long, starting with time for meet and greet, followed by two or three
talks of up to 30 minutes each on any topics that we find interesting, followed
by time for networking. Since AOSP and AAOS developers are scattered over a
wide area, this is an online meetup. We use a Meetup.com group to coordinate
the live meetups - https://www.meetup.com/the-aosp-and-aaos-meetup/

* you will get a link to the jitsi session when you RSVP to a meeting

The talks are recorded and available online for those who didn’t make the
meeting, and also to create an archive of useful information.

TODOs: rework content

## Joining a meetup

* describe the new process: discord and email instead of meetup.com

## Events

<ul>
{% for meetup in site.meetup %}
  <li>
    <a href="{{ meetup.url }}">{{meetup.title}}</a>
  </li>
{% endfor %}
</ul>


## History

TODO some words about the history, e.g. the other domain.
