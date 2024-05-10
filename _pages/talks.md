---
layout: archive
title: "Talks"
permalink: /talks/
author_profile: true
# header:
#  og_image: "research/IMG0102_resize.PNG"
---

Yiheng has been invited to speak at several events, including a university commencement, career development panels, and guest lectures on Machine Learning and AI. He also runs workshops that help business students and executives build data literacy and stay current with the latest trends in Analytics, Data Science, and AI.


<nbsp>

{% include base_path %}

{% assign ordered_pages = site.talks | sort:"order_number" %}

{% for post in ordered_pages %}
  {% include archive-single-talk.html type="grid" %}
{% endfor %}
