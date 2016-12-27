---
layout: default
title: Blog
---
## Welcome to my blog 
I often write blogposts, either contributing to other blogs or venues, such as DiXiT-blog, or original ones. As I am writing and thinking both in English and (originally) in Greek, I don't translate my blogposts.<br/>
Φυσικά, μιλάω και (κυρίως σκεφτομαι) Ελληνικά. Αγαπώ και τις δυο γλώσσες, γι' αυτό και δεν μεταφράζω.

<br/>
<hr/>

{% for post in site.posts %}

<h2><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></h2>

<p class="kicker">{{post.date | date: "%B %-d, %Y"}}</p>
<br/>
{{ post.excerpt | remove: '</p>' }} <a href="{{ site.url }}{{ post.url }}">Read the full post &raquo;</a></p>
<hr/>
{% endfor %}
