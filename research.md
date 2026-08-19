---
layout: page
title: Research
permalink: /research/
---
We seek to understand how alternative splicing and other post-transcriptional RNA processes shape gene expression, and how this mediates genetic variation to human disease. We develop statistical and computational methods, spanning single-cell to population-scale data, and apply them to uncover the regulatory logic of the transcriptome.

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

<p class="profile__note">
  <strong>About my name:</strong> I am always grateful to see people cite my papers!
  If you do, please note that <strong>Buen Abad</strong> is part of a compound surname (not a middle name),
  so the correct citation format is <strong>Buen Abad Najar, C.F.</strong> Reference managers often
  split it incorrectly into Najar, C.F.B.A. Please consider correcting this if you notice it.
</p>
<p class="profile__note">
  For informal purposes, you can abbreviate my name to Carlos <strong>Buen Abad</strong>.
</p>

