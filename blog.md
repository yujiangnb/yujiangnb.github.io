---
layout: blog
title: Blog
permalink: /blog/
---

<h1> Recent Posts </h1>
<ul>
{% for notes in site.posts limit:5%}
<li>
  {{notes.date | date: '%D'}} <a href="{{site.baseurl}}{{ notes.url }}">{{ notes.title }}</a>
  <p>{{notes.content}}</p>
</li>
{% endfor %}
</ul>