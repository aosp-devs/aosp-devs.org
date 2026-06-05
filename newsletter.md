---
layout: default
---

# aosp-devs.org Newsletters

List of all published newsletters (latest at the top):

{% for post in site.posts %}
{% if post.categories contains "newsletter" %}
<p>
  <a href="{{ post.url }}">{{ post.date | date: "%Y" }} {{ post.title }}</a>
</p>
{% endif %}
{% endfor %}
