---
layout: single
title: "Gallery"
permalink: /gallery/
author_profile: true
---

Welcome to my photo gallery. Replace these sample images with your own photographs.


<div class="gallery">
  <figure>
    <img src="/images/gallery/Tampa.jpg" alt="Tampa">
    <figcaption>Tampa, FL – July 2025</figcaption>
  </figure>
  <figure>
    <img src="/images/gallery/Dallas.jpg" alt="Dallas">
    <figcaption>Dallas, TX – April 2023</figcaption>
  </figure>
  <figure>
    <img src="/images/gallery/Charlotte.jpg" alt="Charlotte">
    <figcaption>Charlotte, NC – Auguest 2022</figcaption>
  </figure>
</div>

<style>
.gallery {
  display: grid;
  grid-template-columns: repeat(3, 1fr); /* fixed 3 columns */
  gap: 1rem;
}

.gallery img {
  width: 100%;
  aspect-ratio: 1 / 1; /* make it square */
  object-fit: cover;   /* crop to fit the square */
  display: block;
  border-radius: 6px; /* optional for rounded corners */
}

figure {
  margin: 0;
  text-align: center;
}

figcaption {
  left: 50%;
  margin-top: 0.5rem;
  font-size: 0.9rem;
  color: #555;
}
</style>