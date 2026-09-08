---
layout: page
title: Exhibition
permalink: /exhibition/
image: '/images/museum-exhibition.jpg'
description: 'Duyên Linh: The Imprint of Buddhism Across Time'
---

**Duyên Linh: The Imprint of Buddhism Across Time** <br />
<i>Curators: Hoàng Ngọc An and Stephen Christopher</i>

Hosted at Hải An Gallery in Hồ Chí Minh City from March to May 2026, this 45-day exhibition now continues online as a virtual experience. Duyên Linh traced the emergence of Tibetan Buddhism in Vietnam through temple statues, scroll paintings, prayer flags, monastic robes, and digital media.

Organized around five Buddhist ideas – navigating, attracting, emitting, spinning, and tying – the exhibition explored how emergent Tibetan Buddhism takes shape in everyday Vietnamese life through personal stories, lived experiences, and creative expressions of faith.

Resources related to the exhibition include:
- A 3D walkthrough featuring hundreds of interactive artworks, accompanied by a soundtrack of Tibetan-Vietnamese LOFI music.
- An educational resource packet for introductory college courses, featuring activities and supplementary information designed to deepen engagement with the exhibition.
- A series of ethnographic short films commissioned for the exhibition, presenting the research underlying the exhibition.
- Publications associated with the exhibition, including an article in Museum Anthropology, a research catalogue published by Vajra Academic, and an article in #AsiaNow, the blog of the Association for Asian Studies.

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
<summary>Educational Resource Packet</summary>

An educational resource for introductory college courses in religious studies, anthropology, Vietnamese studies, and Tibetan studies, designed to complement the exhibition.

<p><a class="button button--primary" href="{{ site.baseurl }}/files/DUYEN-LINH-Educational-Packet.pdf" download>Download PDF</a></p>

<iframe src="{{ site.baseurl }}/files/DUYEN-LINH-Educational-Packet.pdf" class="pdf-embed" title="Educational Resource Packet"></iframe>

</details>

<details name="exhibition" class="exhibition-section" markdown="1">
<summary>Ethnographic Short Films</summary>

Twelve short films documenting contemporary religious communities, produced as part of the exhibition. Videos will be added here as they become available.

{% assign film_ids = "1O4ubiKAFqc,83oPuyzR8_4,DM9sPAALxpo,ua01aVtyLD8,eb52VqH4z4U,PmFb0o8lGcI,4Du7EafqN3s,2bF3WTNFr6E,sv6IE2EnuEg,w9TKBDK0Xj0" | split: "," %}
{% assign film_titles = "Thich Minh Tinh,DaoMau,Fire Puja,BoHa,Ogen,LanAnh,Sculptors,Lam Hue Temple,Viet Nam Vajrayana,Duyen Linh Exhibition 2026" | split: "," %}
<div class="video-grid">
{% for i in (1..12) %}
  <div class="video-grid__item">
    <div class="video-grid__frame">
      {% assign video_id = film_ids[forloop.index0] %}
      {% assign video_title = film_titles[forloop.index0] %}
      {% if video_id %}
      <div class="yt-facade" data-id="{{ video_id }}" data-title="{{ video_title }}">
        <img class="yt-facade__thumb" loading="lazy" src="https://i.ytimg.com/vi/{{ video_id }}/hqdefault.jpg" alt="{{ video_title }}">
        <div class="yt-facade__overlay">
          <div class="yt-facade__text">
            <span class="yt-facade__title">{{ video_title }}</span>
            <span class="yt-facade__channel">Duyen Linh Exhibition</span>
          </div>
          <button type="button" class="yt-facade__play" aria-label="Play {{ video_title }}" onclick="var f=document.createElement('iframe');f.src='https://www.youtube-nocookie.com/embed/{{ video_id }}?autoplay=1&rel=0&modestbranding=1';f.title='{{ video_title }}';f.frameBorder='0';f.allow='autoplay; encrypted-media';f.allowFullscreen=true;this.parentElement.parentElement.replaceWith(f);"></button>
        </div>
      </div>
      {% else %}
      <p class="video-grid__placeholder">Film {{ i }}<br>Coming soon</p>
      {% endif %}
    </div>
  </div>
{% endfor %}
</div>

</details>

<details name="exhibition" class="exhibition-section" markdown="1">
<summary>Publications</summary>

<div class="publication-category">
<h2>Article — Museum Anthropology</h2>
<p class="forthcoming">Forthcoming</p>
</div>

<div class="publication-category">
<h2>Research Catalogue — Vajra Academic</h2>
<p class="forthcoming">Forthcoming</p>
</div>

<div class="publication-category">
<h2>Article — #AsiaNow (Association for Asian Studies blog)</h2>
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
.yt-facade {
  position: absolute;
  inset: 0;
}
.yt-facade__thumb {
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.yt-facade__overlay {
  position: absolute;
  inset: 0;
  background: linear-gradient(180deg, rgba(0,0,0,0.55) 0%, rgba(0,0,0,0) 35%, rgba(0,0,0,0) 60%, rgba(0,0,0,0.6) 100%);
}
.yt-facade__text {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  padding: 12px 16px;
  color: #fff;
}
.yt-facade__title {
  display: block;
  font-weight: 700;
  font-size: 1em;
  text-shadow: 0 1px 3px rgba(0,0,0,0.6);
}
.yt-facade__channel {
  display: block;
  font-size: 0.8em;
  opacity: 0.85;
  text-shadow: 0 1px 3px rgba(0,0,0,0.6);
}
.yt-facade__play {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 56px;
  height: 40px;
  border: 0;
  border-radius: 8px;
  background: #FF0000;
  cursor: pointer;
}
.yt-facade__play::after {
  content: "";
  position: absolute;
  top: 50%;
  left: 54%;
  transform: translate(-50%, -50%);
  border-style: solid;
  border-width: 8px 0 8px 14px;
  border-color: transparent transparent transparent #fff;
}
.yt-facade__play:hover {
  background: #e60000;
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
