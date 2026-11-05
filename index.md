---
layout: default
---

# Ebrahim Aliabadi Farahani

I'm a research data scientist at Google. I received my PhD in economics from
the University of Texas at Austin.

My research is in mechanism design, auctions, and the economics of
marketplaces. Lately I've been focused on what happens when AI agents interact
with one another.

## Research {#research}

<!-- Papers are listed in _data/papers.yml (see the instructions at the top of that file). -->

{% for paper in site.data.papers %}
<div class="paper">
  <h3><a href="{{ '/papers/' | append: paper.id | append: '/' | relative_url }}">{{ paper.title }}</a></h3>
  <p class="venue">{{ paper.status }}</p>
  <p>{{ paper.abstract }}</p>
  <p class="paper-links">
    <a href="{{ paper.pdf | relative_url }}">PDF</a>
    {% if paper.ssrn %}<a href="{{ paper.ssrn }}">SSRN</a>{% endif %}
  </p>
</div>
{% endfor %}
