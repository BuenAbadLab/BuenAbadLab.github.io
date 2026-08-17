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

### Earlier work

<ul class="pub-list">
  <li class="pub-list__item">
    <span class="pub-list__year">2015</span>
    <span class="pub-list__entry">Vohr S, Buen Abad Najar CF, Shapiro B, Green RE. <strong>A method for positive forensic identification of samples from extremely low-coverage sequence data.</strong> <em>BMC Genomics</em> 16:1034.</span>
  </li>
  <li class="pub-list__item">
    <span class="pub-list__year">2015</span>
    <span class="pub-list__entry">Sankoff D, Zheng C, Wang B, Buen Abad Najar CF. <strong>Structural vs. functional mechanisms of duplicate gene loss following whole genome doubling.</strong> <em>BMC Bioinformatics</em> 16(Suppl 17):S9.</span>
  </li>
  <li class="pub-list__item">
    <span class="pub-list__year">2013</span>
    <span class="pub-list__entry">Chen ECH, Buen Abad Najar CF, Zheng C, et al. <strong>The dynamics of functional classes of plant genes in rediploidized ancient polyploids.</strong> <em>BMC Bioinformatics</em> 14(Suppl 15):S19.</span>
  </li>
</ul>
