---
layout: page
permalink: /works/index.html
title: 许德民作品
tagline: Minimal Mistakes, a Jekyll Theme
tags: [about, Jekyll, theme, responsive]
modified: 9-9-2013
image:
  feature: texture-feature-02.jpg
  credit: Texture Lovers
  creditlink: http://texturelovers.com
images-s1:
  - 1.jpg
  - 2.jpg
images-s2:
  - 3.jpg
  - 4.jpg
images-s3:
  - 5.jpg
  - 6.jpg
imageroot: /assets/images/works/series1/fullsize
---
<script src="{{ site.url }}/assets/js/vendor/picturefill.js"></script>
<script src="{{ site.url }}/assets/js/vendor/jquery-1.9.1.min.js"></script>
<script src="{{ site.url }}/assets/js/vendor/galleria/galleria-1.3.3.js"></script>
<link rel="stylesheet" href="{{ site.url }}/assets/js/vendor/galleria/themes/classic/galleria.classic.css">
<!-- <link rel="stylesheet" href="/assets/js/vendor/galleria/themes/twelve/galleria.twelve.css"> -->
<style>
    .galleria-classic{ width: 700px; height: 400px; background: #000 }
</style>

## 作品系列一：
<div class="galleria-classic">
{% for image in page.images-s1 %}
  <img src="{{ site.url }}/{{ page.imageroot }}/{{image}}">
{% endfor %}
</div>

## 作品系列二：
<div class="galleria-classic">
{% for image in page.images-s2 %}
  <img src="{{ site.url }}/{{page.imageroot}}/{{image}}">
{% endfor %}
</div>

## 作品系列三：
<div class="galleria-classic">
{% for image in page.images-s3 %}
  <img src="{{ site.url }}/{{page.imageroot}}/{{image}}">
{% endfor %}
</div>
<script>
Galleria.configure({
    lightbox: true,
    carousel: true
});

Galleria.loadTheme('{{ site.url }}/assets/js/vendor/galleria/themes/classic/galleria.classic.min.js');
Galleria.run('.galleria-classic');  

// Galleria.loadTheme('/assets/js/vendor/galleria/themes/twelve/galleria.twelve.js');
// Galleria.run('.galleria-twelve');  

// debugger;
</script>
