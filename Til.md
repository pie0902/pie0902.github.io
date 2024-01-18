---
layout: post
title: "Today I Learned"
categories: [Til]
---
{% for post in site.posts %}
{% if post.categories contains 'Til' %}
<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
<p>{{ post.excerpt }}</p>
{% endif %}
{% endfor %}