---
title: "Home"
layout: homelay
permalink: /
---

<h1 class="home-hero">{{ site.name }}</h1>
<p class="home-hero-sub">{{ site.title }}, {{ site.institution }}</p>

<div class="chip-container" markdown="0">
<a href="{{ '/research' | relative_url }}" class="chip">Seismic Imaging</a>
<a href="{{ '/research' | relative_url }}" class="chip">Marchenko Methods</a>
<a href="{{ '/research' | relative_url }}" class="chip">Wave Propagation</a>
<a href="{{ '/research' | relative_url }}" class="chip">Machine Learning</a>
<a href="{{ '/research' | relative_url }}" class="chip">Carbon Storage Monitoring</a>
</div>

I am a geophysicist working at the intersection of seismic wave propagation, subsurface imaging, and machine learning. My research develops data-driven methods that make complex seismic signals more useful for imaging and monitoring the subsurface.

<div class="callout callout-success" markdown="0">
<div class="callout-title">Research focus</div>
<p>Marchenko redatuming and focusing, multiple attenuation and deghosting, seismic interferometry, and machine-learning methods for seismic processing.</p>
</div>

{% capture selected %}{% bibliography --query @*[selected=true] %}{% endcapture %}
{% if selected contains "pub-entry" %}
## Selected publications

<div class="section-card selected-pubs" markdown="0">
{{ selected }}
<p style="margin: var(--space-4) 0 0;"><a href="{{ '/publications' | relative_url }}">All publications &rarr;</a></p>
</div>
{% endif %}

## About me

I earned my Ph.D. in Geophysics from Colorado School of Mines in 2023, where my doctoral research focused on data-driven and machine-learning approaches for suppressing multiply reflected seismic waves. Earlier, I completed an M.S. in Geophysics at Purdue University, studying Marchenko redatuming and imaging for carbon sequestration monitoring. I am currently affiliated with ExxonMobil in the Houston area.

My work combines physical modeling with modern computational methods to improve seismic imaging, noise attenuation, and subsurface monitoring. See the [research page]({{ '/research' | relative_url }}) for an overview and [publications]({{ '/publications' | relative_url }}) for peer-reviewed work.
