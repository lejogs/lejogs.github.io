---
layout: page
title: Pedalling rubbish
tagline: 4 guys, 1000 miles, 12 days... no idea
---
{% include JB/setup %}

Welcome - we're gearing up to the challenge of cycling the 1000 miles from Land's End to John O'Groats.
We'd love you to [sponsor](http://lejo.gs/sponsor) us! In the meantime - this is what's keeping us busy:

###Latest Articles

<ul>
{% for post in site.posts limit:5 %}
                    <dt>
                        <hgroup>
                            <a class="title" href="{{ post.url }}">{{ post.title }}</a>
                            <time class="date" datetime="{{ post.date | date_to_string }}" pubdate="pubdate">{{ post.date | date: '%B %d, %Y' }}</time>
                        </hgroup>
                    </dt>
                              <dd>
                    {{ post.content | truncatewords 12 }} <a href="{{post.url}}" class="more-link">Read more.</a>
                              </dd>
{% endfor %}
</ul>
