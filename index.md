---
layout: page
title: Home
tagline: Microsoft MVP, Please Notice Me!
---
{% include JB/setup %}

## About

My name is `John Crowe` and I am a software developer and consultant at Sogeti USA.
    
## Recent Posts

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
