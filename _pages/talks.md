---
layout: archive
title: "Talks"
permalink: /talks/
author_profile: true
# header:
#  og_image: "research/IMG0102_resize.PNG"
---

Yiheng has spoken at university commencements, career development events, and is the creator of several tutorial workshops on topics related to Economics, Data Analytics, Business Intelligence, and AI for business students.

<nbsp>

{% include base_path %}

{% assign ordered_pages = site.talks | sort:"order_number" %}

{% for post in ordered_pages %}
  {% include archive-single.html type="grid" %}
{% endfor %}
