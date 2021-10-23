---
layout: page
title: DS
permalink: /Data Science/
description: Sort my blog posts by topic.
---
<header class="major">
  <h2><a href="#">Blog Posts by Topic</a></h2>
</header>
<p>
<div class="row">
  <div class="6u 12u$(small)">
    {% for category in site.tags %}
    {% capture category_name %}{{ category | first }}{% endcapture %}

    <h3>{{ category_name }}</h3>
    <a name="{{ category_name | slugize }}"></a>
    <ul>
      {% for post in site.tags[category_name] %}
        {% if post.external_url %}
          <li><a href="{{ post.external_url }}" rel="canonical" target="blank">{{post.title}}</a></li>
        {% else %}
          <li><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></li>
        {% endif %}
      {% endfor %}
    </ul>
    {% endfor %}
  </div></div>
