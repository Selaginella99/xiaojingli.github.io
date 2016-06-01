---
layout: archive
permalink: /tags/
title: "Posts by Tags"
author_profile: false

excerpt: "按照标签分类"
header:
  overlay_image: computer.jpg
  teaser: "computer.jpg"
  overlay_filter: 0.5 # same as adding an opacity of 0.5 to a black background
---

{% include base_path %}
{% include group-by-array collection=site.posts field="tags" %}

{% for tag in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  <h2 id="{{ tag | slugify }}" class="archive__subtitle">{{ tag }}</h2>
  {% for post in posts %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}