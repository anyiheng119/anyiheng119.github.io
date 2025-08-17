---
layout: single
title: "Gallery"
permalink: /gallery/
author_profile: true
---

I love exploring new places — each journey gives me space to reflect, imagine, and see the world from fresh perspectives.

<div class="gallery">
  <div class="gallery-item">
    <img src="/images/gallery/Tampa.jpg" alt="Tampa">
    <div class="caption">Tampa, FL – July 2025</div>
  </div>

  <div class="gallery-item">
    <img src="/images/gallery/Dallas.jpg" alt="Dallas">
    <div class="caption">Dallas, TX – April 2023</div>
  </div>

  <div class="gallery-item">
    <img src="/images/gallery/Charlotte.jpg" alt="Charlotte">
    <div class="caption">Charlotte, NC – Auguest 2022</div>
  </div>
</div>

<style>
.gallery {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr)); /* fixed 3 columns */
  gap: 1rem;
}

.gallery img {
  width: 100%;
  aspect-ratio: 1 / 1; /* make it square */
  object-fit: cover;   /* crop to fit the square */
  display: block;
  border-radius: 6px; /* optional for rounded corners */
}

.gallery-item {
  text-align: center; /* centers everything inside, including .caption */
}

figure {
  margin: 0;
  text-align: center;
}

caption {
  margin-top: 0.5rem;
  font-size: 0.9rem;
  color: #555;
  text-align: center;
}
</style>