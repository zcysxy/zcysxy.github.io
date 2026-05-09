---
layout: archive
title: "Research"
permalink: /research/
author_profile: false
---

I help machines efficiently learn how to make decisions.

My long-term research goal is to combine efficient optimization methods and tailored machine learning frameworks with strong theoretical guarantees to address societal challenges.

```mermaid
%%{init: {'theme': 'base', 'themeVariables': { 'primaryColor': '#00876255'}}}%%
flowchart LR
A[Societal Challenges] <--> B
  B[Machine Learning] <--> C
    C[Efficient Optimization] <--> D
      D[Mathematical Insights]
```

With this goal in mind, my current research interests are in **decision-making** (reinforcement learning & control), **multi-agent machine learning** (federated learning & game), and **optimization**.

## Publications {% if site.author.googlescholar %}[[Google Scholar]({{site.author.googlescholar}})]{% endif %}

{% include base_path %}

<!-- New style rendering if publication categories are defined -->
{% comment %}
{% raw %}
{% if site.publication_category %}
  {% for category in site.publication_category  %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
## {{ category[1].title }}
___
        {% assign title_shown = true %}
      {% endunless %}
      {% include archive-single.html %}
    {% endfor %}
  {% endfor %}
{% else %}
{% endraw %}
{% endcomment %}

{% for post in site.publications reversed %}
{% include archive-single.html %}
{% endfor %}

{% comment %}
{% raw %}
{% endif %}
{% endraw %}
{% endcomment %}



