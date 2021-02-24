---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
Most of these publications may also be found on my <u><a href="https://scholar.google.com/citations?user=NZVGPiwAAAAJ&hl=en&oi=ao">google scholar profile</a>.</u>
<br>If you like the format of the preprints included here, see <u><a href="https://github.com/brenhinkeller/preprint-template.tex">preprint-template.tex</a></u>

---
{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

