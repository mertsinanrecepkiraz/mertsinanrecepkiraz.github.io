---
title: "Publications"
layout: page
permalink: /publications/
---

# Publications

<div class="publication-page" id="pubList">
<section class="publication-section" aria-labelledby="articles-heading">
<h2 id="articles-heading">Articles</h2>

{% bibliography --query @article %}
</section>

<section class="publication-section" aria-labelledby="thesis-heading">
<h2 id="thesis-heading">Thesis</h2>

{% bibliography --query @*[category=thesis] %}
</section>

<section class="publication-section" aria-labelledby="proceedings-heading">
<h2 id="proceedings-heading">Refereed Conference Proceedings</h2>

{% bibliography --query @inproceedings %}
</section>
</div>
