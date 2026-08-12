---
layout: page
title: Ethnographic Short Films
permalink: /exhibition/films/
image: '/images/museum-exhibition.jpg'
description: 'Twelve ethnographic short films documenting contemporary religious communities'
---

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
</style>
