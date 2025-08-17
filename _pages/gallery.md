---
layout: single
title: "<p align='center'><font size='+3'><b>Gallery</b></font></p>"
permalink: /gallery/
author_profile: false
---

Welcome to my photo gallery. Replace these sample images with your own photographs.

<div class="gallery">
  <figure>
    <img src="https://picsum.photos/id/1025/600/400" alt="Puppy">
    <figcaption>Puppy – July 2025</figcaption>
  </figure>
  <figure>
    <img src="https://picsum.photos/id/1003/600/400" alt="Ocean view">
    <figcaption>Ocean view – June 2025</figcaption>
  </figure>
  <figure>
    <img src="https://picsum.photos/id/1015/600/400" alt="Mountain">
    <figcaption>Mountain – May 2025</figcaption>
  </figure>
</div>

<style>
.gallery {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  gap: 1rem;
}
.gallery img {
  width: 100%;
  height: auto;
  display: block;
}
figure {
  margin: 0;
}
figcaption {
  text-align: center;
  margin-top: 0.5rem;
  font-size: 0.9rem;
  color: #555;
}
</style>
