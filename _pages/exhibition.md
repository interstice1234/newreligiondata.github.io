---
layout: page
title: Exhibition
permalink: /exhibition/
image: '/images/museum-exhibition.jpg'
description: 'Exhibition on new religious movements and human flourishing'
---

Explore the project's museum exhibition on new religious movements and human flourishing through four sections:

* [Ethnographic Short Films](#films) — 12 short films documenting contemporary religious communities
* [Educational Resource Packet](#packet) — a 50-page classroom resource
* [3D Walkthrough](#walkthrough) — an interactive virtual tour of the exhibition
* [Publications](#publications) — articles and books related to the exhibition

***

## Ethnographic Short Films {#films}

Twelve short films documenting contemporary religious communities, produced as part of the exhibition. Videos will be added here as they become available.

<div class="video-grid">
{% for i in (1..12) %}
  <div class="video-grid__item">
    <div class="video-grid__frame">
      <p class="video-grid__placeholder">Film {{ i }}<br>Coming soon</p>
      <!-- Replace the placeholder above with, e.g.:
      <iframe src="https://www.youtube.com/embed/VIDEO_ID" loading="lazy" frameborder="0" allowfullscreen></iframe>
      -->
    </div>
  </div>
{% endfor %}
</div>

***

## Educational Resource Packet {#packet}

A 50-page educational resource packet prepared for the exhibition.

<p><a class="button button--primary" href="{{ site.baseurl }}/files/DUYEN-LINH-Educational-Packet.pdf" download>Download PDF</a></p>

<iframe src="{{ site.baseurl }}/files/DUYEN-LINH-Educational-Packet.pdf" class="pdf-embed" title="Educational Resource Packet"></iframe>

***

## 3D Walkthrough {#walkthrough}

Explore the exhibition in an interactive 3D walkthrough.

<p><a class="button button--primary" href="https://exhibition.newreligiosity.org/" target="_blank" rel="noopener">Open 3D Walkthrough in a new tab</a></p>

<iframe src="https://exhibition.newreligiosity.org/" class="walkthrough-embed" title="3D Exhibition Walkthrough" allowfullscreen></iframe>
<p class="walkthrough-note">If the walkthrough does not load above, use the link to open it directly.</p>

***

## Publications {#publications}

<div class="publication-category">
<h2>Article</h2>
<p class="forthcoming">Forthcoming</p>
</div>

<div class="publication-category">
<h2>Book — Vajra Academic</h2>
<p class="forthcoming">Forthcoming</p>
</div>

<style>
.video-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 24px;
  margin-top: 24px;
}
.video-grid__frame {
  position: relative;
  aspect-ratio: 16 / 9;
  background: var(--background-alt-color);
  border-radius: 8px;
  overflow: hidden;
}
.video-grid__frame iframe {
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
  border: 0;
}
.video-grid__placeholder {
  position: absolute;
  inset: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  margin: 0;
  color: var(--text-color-light, inherit);
  opacity: 0.6;
}
.pdf-embed {
  width: 100%;
  height: 90vh;
  border: 1px solid var(--border-color, #ccc);
  border-radius: 8px;
  margin-top: 16px;
}
.walkthrough-embed {
  width: 100%;
  height: 80vh;
  border: 1px solid var(--border-color, #ccc);
  border-radius: 8px;
  margin-top: 16px;
}
.walkthrough-note {
  opacity: 0.6;
  font-size: 0.9em;
}
</style>
