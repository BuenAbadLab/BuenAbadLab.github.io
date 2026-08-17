---
layout: page
title: Publications
permalink: /publications/
---
For the most up-to-date list, see [Google Scholar]({{ site.scholar_url }}) or [ORCID]({{ site.orcid_url }}).

<ul class="pub-list">
{%- for pub in site.data.publications -%}
<li class="pub-list__item">
  <span class="pub-list__year">{{ pub.year }}</span>
  <span class="pub-list__entry">
    {{ pub.authors }}. <strong>{{ pub.title }}.</strong> <em>{{ pub.venue }}</em>{% if pub.notes %}. <span class="pub-card__notes">{{ pub.notes }}</span>{% endif %}
    {%- if pub.paper %} &middot; <a href="{{ pub.paper }}">paper</a>{% endif -%}
    {%- if pub.preprint %} &middot; <a href="{{ pub.preprint | relative_url }}">preprint</a>{% endif -%}
    {%- if pub.code %} &middot; <a href="{{ pub.code }}">code</a>{% endif -%}
  </span>
</li>
{%- endfor -%}
</ul>

