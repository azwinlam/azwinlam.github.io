---
layout: archive
title: "Blog"
permalink: /blog/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my blog on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.blog reversed %}
  {% include archive-single.html %}
{% endfor %}