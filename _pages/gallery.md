---
layout: single
title: ""
permalink: /gallery/
author_profile: true
share: false
---

***A visual record of my journey across different cities👇***

---

### Montreal, QC, Canada <span style="font-weight: normal; font-style: italic;">(2026 – Present)</span>

*(Photos TBD)*

---

### Rochester, NY, United States <span style="font-weight: normal; font-style: italic;">(2024 – 2026)</span>

<div class="photo-gallery" id="gallery-rochester">
  <a href="/images/rochester1.jpg"><img src="/images/rochester1.jpg" alt="Rochester 1"></a>
  <a href="/images/rochester2.jpg"><img src="/images/rochester2.jpg" alt="Rochester 2"></a>
  <a href="/images/rochester3.jpg"><img src="/images/rochester3.jpg" alt="Rochester 3"></a>
  <a href="/images/rochester4.jpg"><img src="/images/rochester4.jpg" alt="Rochester 4"></a>
</div>

---

### Macao S.A.R. <span style="font-weight: normal; font-style: italic;">(2019 – 2024)</span>

<div class="photo-gallery" id="gallery-macao">
  <a href="/images/macao1.jpg"><img src="/images/macao1.jpg" alt="Macao 1"></a>
  <a href="/images/macao2.jpg"><img src="/images/macao2.jpg" alt="Macao 2"></a>
  <a href="/images/macao3.jpg"><img src="/images/macao3.jpg" alt="Macao 3"></a>
  <a href="/images/macao4.jpg"><img src="/images/macao4.jpg" alt="Macao 4"></a>
  <a href="/images/macao5.jpg"><img src="/images/macao5.jpg" alt="Macao 5"></a>
</div>

---

### Hefei, Anhui, China <span style="font-weight: normal; font-style: italic;">(Hometown)</span>

<div class="photo-gallery" id="gallery-hefei">
  <a href="/images/hefei1.jpg"><img src="/images/hefei1.jpg" alt="Hefei 1"></a>
  <a href="/images/hefei2.jpg"><img src="/images/hefei2.jpg" alt="Hefei 2"></a>
</div>

<script type="module" markdown="0">
import PhotoSwipeLightbox from 'https://cdn.jsdelivr.net/npm/photoswipe@5.4.4/dist/photoswipe-lightbox.esm.js';

document.addEventListener("DOMContentLoaded", () => {
  const galleryLinks = document.querySelectorAll('.photo-gallery a');
  galleryLinks.forEach(link => {
    const img = link.querySelector('img');
    if (img) {
      if (img.complete) {
        link.setAttribute('data-pswp-width', img.naturalWidth || 1200);
        link.setAttribute('data-pswp-height', img.naturalHeight || 800);
      } else {
        img.onload = () => {
          link.setAttribute('data-pswp-width', img.naturalWidth || 1200);
          link.setAttribute('data-pswp-height', img.naturalHeight || 800);
        };
      }
    }
  });

  const lightbox = new PhotoSwipeLightbox({
    gallery: '.photo-gallery',
    children: 'a',
    pswpModule: () => import('https://cdn.jsdelivr.net/npm/photoswipe@5.4.4/dist/photoswipe.esm.js')
  });
  lightbox.init();
});
</script>
