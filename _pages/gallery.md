---
permalink: /
title: "<p align='center'><font size='+3'><b>Gallery</b></font></p>"
excerpt: "Yiheng An - Personal Website"
author_profile: true
redirect_from: 
  - /gallery/
  - /gallery.html
---

<!-- Intro text -->
<header>
  <h1>Memorable Moments</h1>
  <p class="lede">A lightweight photo gallery page with just a heading and an image grid—no sidebars, no fuss. Replace the sample images below with your own and edit this paragraph to add any intro text you want.</p>
</header>

<div class="bar"></div>

<!-- Image Grid -->
<section class="gallery" id="gallery">
  <figure class="tile">
    <button aria-label="Open image: Magic Touch~ (July 2025)">
      <img class="thumb" loading="lazy" src="https://picsum.photos/id/1025/600/600" alt="Magic Touch~" data-full="https://picsum.photos/id/1025/1600/1200" data-title="Magic Touch~" data-meta="July 2025 · Orlando" />
    </button>
    <figcaption class="caption"><strong>Magic Touch~</strong><span>July 2025 · Orlando</span></figcaption>
  </figure>

  <figure class="tile">
    <button aria-label="Open image: A Doorstep of Love~ (June 2025)">
      <img class="thumb" loading="lazy" src="https://picsum.photos/id/1003/600/600" alt="A Doorstep of Love~" data-full="https://picsum.photos/id/1003/1600/1200" data-title="A Doorstep of Love~" data-meta="June 2025 · Crescent Hill" />
    </button>
    <figcaption class="caption"><strong>A Doorstep of Love~</strong><span>June 2025 · Crescent Hill</span></figcaption>
  </figure>

  <!-- Add more figures as needed -->
</section>

<!-- Lightbox Modal -->
<div class="lightbox" id="lightbox" aria-modal="true" role="dialog" aria-label="Image viewer">
  <div class="frame">
    <button class="closeBtn" id="closeBtn" aria-label="Close"></button>
    <img id="fullImg" alt="" />
    <div class="meta" id="meta"></div>
  </div>
</div>

<footer>
  <small>Built with plain HTML/CSS + tiny JS. Replace placeholders with your own photos under <code>/assets/gallery/</code>.</small>
</footer>

<style>
  :root { --bg:#0b0c10; --panel:#121418; --text:#e9edf1; --muted:#b9c2cc; --accent:#6aa9ff; --ring:rgba(106,169,255,0.35); }
  *{box-sizing:border-box;} html,body{margin:0;padding:0;background:var(--bg);color:var(--text);font:16px/1.6 system-ui,-apple-system,Segoe UI,Roboto,Arial,sans-serif;}
  .wrap{max-width:1100px;margin:0 auto;padding:24px;}
  header{text-align:center;padding:32px 0 8px;} header h1{margin:0 0 8px;font-size:clamp(28px,3.5vw,40px);} header p.lede{margin:0 auto;max-width:70ch;color:var(--muted);}
  .bar{height:1px;background:linear-gradient(90deg,transparent,var(--ring),transparent);margin:24px auto 28px;max-width:640px;}
  .gallery{display:grid;grid-template-columns:repeat(12,1fr);gap:12px;}
  .tile{grid-column:span 6;position:relative;overflow:hidden;border-radius:16px;background:var(--panel);} @media(min-width:640px){.tile{grid-column:span 4;}} @media(min-width:1024px){.tile{grid-column:span 3;}}
  .tile button{all:unset;cursor:zoom-in;display:block;width:100%;height:100%;}
  .thumb{width:100%;height:100%;object-fit:cover;aspect-ratio:1/1;filter:saturate(1.05) contrast(1.02);transition:transform .25s ease;}
  .tile:hover .thumb{transform:scale(1.03);} .caption{position:absolute;left:10px;bottom:10px;right:10px;padding:8px 10px;border-radius:12px;background:linear-gradient(180deg,rgba(0,0,0,0),rgba(0,0,0,.55));color:#fff;font-size:13px;backdrop-filter:blur(2px);}
  .caption strong{display:block;font-weight:600;}.caption span{opacity:.85;}
  .lightbox{position:fixed;inset:0;display:none;place-items:center;background:rgba(5,7,10,0.85);z-index:100;}
  .lightbox.open{display:grid;}.lightbox .frame{position:relative;max-width:92vw;max-height:88vh;}
  .lightbox img{max-width:100%;max-height:88vh;border-radius:14px;box-shadow:0 10px 40px rgba(0,0,0,.5);} .lightbox .meta{margin-top:8px;color:var(--muted);text-align:center;font-size:14px;}
  .closeBtn{position:absolute;top:-12px;right:-12px;background:var(--panel);color:var(--text);width:40px;height:40px;border-radius:999px;cursor:pointer;box-shadow:0 8px 24px rgba(0,0,0,.35);}
  .closeBtn:after{content:"✕";font-size:16px;}
</style>

<script>
  const gallery=document.getElementById('gallery');
  const box=document.getElementById('lightbox');
  const full=document.getElementById('fullImg');
  const meta=document.getElementById('meta');
  const closeBtn=document.getElementById('closeBtn');

  function openLightbox(src,title,info){
    full.src=src;full.alt=title||'';meta.textContent=title?(title+(info?' · '+info:'')):(info||'');
    box.classList.add('open');document.body.style.overflow='hidden';
  }
  function closeLightbox(){box.classList.remove('open');full.src='';document.body.style.overflow='';}

  gallery.addEventListener('click',e=>{const img=e.target.closest('img.thumb');if(!img)return;const src=img.dataset.full||img.src;openLightbox(src,img.dataset.title,img.dataset.meta);});
  box.addEventListener('click',e=>{if(e.target===box)closeLightbox();});
  closeBtn.addEventListener('click',closeLightbox);
  window.addEventListener('keydown',e=>{if(e.key==='Escape')closeLightbox();});
</script>
