---
layout: archive
title: "Bio"
permalink: /bio/
author_profile: true
---

<br style="margin-bottom: 1.5em;" />

{% include base_path %}


<div class="grid__row">
{% for post in site.bio %}
  {% include archive-single.html type="grid" %}
{% endfor %}
</div>

