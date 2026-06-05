---
layout: default
---

<h1>Blog posts</h1>

The blog posts are also availabe as a [RSS feed](/feed.xml):

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.date | date: "%Y-%m" }}:  {{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
