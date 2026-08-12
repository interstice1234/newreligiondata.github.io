---
layout: page
title: Exhibition
permalink: /exhibition/
image: '/images/museum-exhibition.jpg'
description: 'Duyên Linh: The Imprint of Buddhism Across Time'
---

**Duyên Linh: The Imprint of Buddhism Across Time** traces the evolving presence of Tibetan Buddhism in Vietnam, from temple statues and scroll paintings to prayer flags, monk robes, and digital media. Structured around five Buddhist ideas — navigating, attracting, emitting, spinning, and tying — the exhibition shows how these traditions are practiced in everyday life through personal stories, lived experience, and creative expressions of faith. Curated by Hoàng Ngọc An and Stephen Christopher, it was shown at the Hải An Gallery in Hồ Chí Minh City (March–May 2026) and continues here as a virtual exhibition.

<details name="exhibition" class="exhibition-section" markdown="1">
<summary>Ethnographic Short Films</summary>

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

</details>

<details name="exhibition" class="exhibition-section" markdown="1">
<summary>Educational Resource Packet</summary>

A 50-page educational resource packet prepared for the exhibition.

<p><a class="button button--primary" href="{{ site.baseurl }}/files/DUYEN-LINH-Educational-Packet.pdf" download>Download PDF</a></p>

<iframe src="{{ site.baseurl }}/files/DUYEN-LINH-Educational-Packet.pdf" class="pdf-embed" title="Educational Resource Packet"></iframe>

</details>

<details name="exhibition" class="exhibition-section" markdown="1">
<summary>3D Walkthrough</summary>

Explore the exhibition in an interactive 3D walkthrough. It plays audio, so it only loads once you press play below.

<p><a class="button button--primary" href="https://exhibition.newreligiosity.org/" target="_blank" rel="noopener">Open 3D Walkthrough in a new tab</a></p>

<div class="walkthrough-embed">
  <button type="button" class="walkthrough-play" onclick="var f=document.createElement('iframe');f.src='https://exhibition.newreligiosity.org/';f.title='3D Exhibition Walkthrough';f.className='walkthrough-embed';f.allowFullscreen=true;this.parentElement.replaceWith(f);">▶ Play 3D Walkthrough</button>
</div>
<p class="walkthrough-note">Includes audio — starts only when you press play.</p>

</details>

<details name="exhibition" class="exhibition-section" markdown="1">
<summary>Publications</summary>

<div class="publication-category">
<h2>Article</h2>
<p class="forthcoming">Forthcoming</p>
</div>

<div class="publication-category">
<h2>Book — Vajra Academic</h2>
<p class="forthcoming">Forthcoming</p>
</div>

</details>

<style>
.exhibition-section {
  border: 1px solid var(--border-color);
  border-radius: var(--global-radius, 8px);
  padding: 20px 24px;
  margin-top: 16px;
  transition: border-color .35s;
}
.exhibition-section[open] {
  border-color: var(--brand-color);
}
.exhibition-section summary {
  cursor: pointer;
  list-style: none;
  display: flex;
  align-items: center;
  justify-content: space-between;
  font-family: var(--heading-font-family, inherit);
  font-size: 1.4em;
  font-weight: 800;
  color: var(--heading-font-color);
}
.exhibition-section summary::-webkit-details-marker { display: none; }
.exhibition-section summary::after {
  content: "+";
  font-size: 1em;
  color: var(--brand-color);
  transition: transform .35s;
  flex: none;
  margin-left: 16px;
}
.exhibition-section[open] summary::after {
  transform: rotate(45deg);
}
.exhibition-section summary:hover {
  color: var(--link-color-hover);
}
.exhibition-section[open] summary {
  margin-bottom: 16px;
  padding-bottom: 16px;
  border-bottom: 1px solid var(--border-color);
}
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
  color: var(--text-alt-color);
  opacity: 0.6;
}
.pdf-embed {
  width: 100%;
  height: 90vh;
  border: 1px solid var(--border-color);
  border-radius: 8px;
  margin-top: 16px;
}
.walkthrough-embed {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 80vh;
  border: 1px solid var(--border-color);
  border-radius: 8px;
  margin-top: 16px;
  background: var(--background-alt-color);
}
iframe.walkthrough-embed {
  display: block;
}
.walkthrough-play {
  padding: 16px 32px;
  font-size: 1.1em;
  cursor: pointer;
  border: 1px solid var(--border-color);
  border-radius: 6px;
  background: transparent;
  color: inherit;
}
.walkthrough-note {
  opacity: 0.6;
  font-size: 0.9em;
}
</style>
