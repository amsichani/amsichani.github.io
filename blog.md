---
layout: default
title: Blog
---
## this is my blog 

<center>Subscribe to the <a href="./feed.xml">RSS feed</a> for new blog posts.</center>
<br/>
<hr/>

{% for post in site.posts %}

<h3><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></h3>

<p class="kicker">{{post.date | date: "%B %-d, %Y"}}</p>
<br/>

{{ post.excerpt | remove: '</p>' }} <a href="{{ site.url }}{{ post.url }}">Read the full post! &raquo;</a></p>

<hr/>

{% endfor %}
