---
permalink: /uber
layout: archive
title: "Posts by Category"
author_profile: false

excerpt: "随便写写"
header:
  overlay_image: computer.jpg
  overlay_filter: 0.5 # same as adding an opacity of 0.5 to a black background
---



{% include base_path %}
{% include group-by-array collection=site.posts field="categories" %}

{% for category in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  <h2 id="{{ category | slugify }}" class="archive__subtitle">{{ category }}</h2>
  {% for post in posts %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}