---
layout: page
title: Research
permalink: /research/
---
Research in the BuenAbad Lab centers on computational RNA biology, genomics, and multi-omics — understanding how RNA splicing and other post-transcriptional processes shape gene expression, and how this connects genetic variation to human disease. We develop statistical and computational methods, spanning single-cell to population-scale data, and apply them to uncover the regulatory logic of the transcriptome.

Below are highlights from our published and ongoing work.

<div class="pub-grid">
{%- for pub in site.data.publications -%}
<div class="pub-card">
  <div class="pub-card__image" style="background-image:url('{{ pub.image | relative_url }}');"></div>
  <div class="pub-card__body">
    <span class="pub-card__venue">{{ pub.venue }}, {{ pub.year }}</span>
    <h3 class="pub-card__title">{{ pub.title }}</h3>
    <p class="pub-card__authors">{{ pub.authors }}{% if pub.notes %}<br><span class="pub-card__notes">{{ pub.notes }}</span>{% endif %}</p>
    <p class="pub-card__desc">{{ pub.description }}</p>
    <p class="pub-card__links">
      {%- if pub.paper %}<a href="{{ pub.paper }}">Paper</a>{% endif -%}
      {%- if pub.preprint %} &middot; <a href="{{ pub.preprint | relative_url }}">Preprint</a>{% endif -%}
      {%- if pub.code %} &middot; <a href="{{ pub.code }}">Code</a>{% endif -%}
    </p>
  </div>
</div>
{%- endfor -%}
</div>
