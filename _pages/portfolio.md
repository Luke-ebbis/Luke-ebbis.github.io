---
layout: archive
title: "portfolio"
permalink: /portfolio/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

My portfolio can also be found on [gitlab](https://git.wur.nl/sibbe.bakker/portfolio).

{% include base_path %}  {% for post in site.portfolio %}  {% include archive-single.html %} {% endfor %}


