---
layout: page
title: Home
tagline: Microsoft MVP, Please Notice Me!
---
{% include JB/setup %}

## About

I'm John Crowe! I'm a entry level software developer and consultant at Sogeti USA. I work and play in Austin, TX. Its a pretty cool deal.
    
## Recent Posts

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
