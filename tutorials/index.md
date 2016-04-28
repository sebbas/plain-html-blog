---
layout: page
title: Tutorials
updated: 2016-04-01 09:00:00 +0200
---
<p>
{% for post in site.categories.tutorials %}
  {% unless post.draft %}
  {% assign currentdate = post.date | date: "%Y" %}
  {% if currentdate != date %}
    {% unless forloop.first %}</ul>{% endunless %}
    <h3>{{ currentdate }}</h3>
    <ul>
    {% assign date = currentdate %}
  {% endif %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
  {% if forloop.last %}</ul>{% endif %}
  {% endunless %}
{% endfor %}
</p>
<p><a href="{{ "/feed.xml" | prepend: site.baseurl }}">RSS</a> feed</p>