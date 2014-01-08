---
layout: page
title: Changes
tagline: Supporting tagline
---
{% include JB/setup %}

## Saddle up

Welcome - we're gearing up to the challenge of cycling the 1000 miles from Land's End to John O'Groats.

We'd love you to [sponsor](http://lejo.gs/sponsor) us!

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
