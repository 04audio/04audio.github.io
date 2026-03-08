---
layout: default
title: 关于
---

<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css" />
<style>
  /* 调整翻页组件的样式，保持和首页一样的大片感 */
  .swiper { width: 100%; padding-bottom: 40px; margin-top: 20px; }
  .swiper-slide { opacity: 0.4; transition: 0.3s; border-radius: 12px; overflow: hidden; background: #000; }
  .swiper-slide-active { opacity: 1; box-shadow: 0 10px 30px rgba(0,0,0,0.5); }
  .v-container { position: relative; padding-bottom: 56.25%; height: 0; }
  .v-container iframe { position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0; }
  .v-label { background: #1a1a1a; padding: 10px 15px; border-top: 1px solid #333; }
  .v-label p { color: #888; font-size: 0.75rem; margin: 0; letter-spacing: 0.5px; }
  .v-label strong { color: #00e5ff; }
  .swiper-button-next, .swiper-button-prev { color: #00e5ff !important; transform: scale(0.5); }
  .swiper-pagination-bullet-active { background: #00e5ff !important; }
</style>

<div style="margin-top: 2rem; margin-bottom: 1.5rem;">
  <h2 style="color: #ffffff; font-size: 0.95rem; font-weight: 800; letter-spacing: 0.5px; text-transform: uppercase; margin: 0;">
    Wwise集成与功能实现
  </h2>
  <p style="color: #888; font-size: 0.85rem; margin-top: 10px;">
    Technical Audio Design & Implementation
  </p>
</div>

<div class="swiper mySwiper">
  <div class="swiper-wrapper">
    <div class="swiper-slide">
      <div class="v-container"><iframe src="//player.bilibili.com/player.html?bvid=BV1vx421C78u&high_quality=1&danmaku=0" scrolling="no" frameborder="no" allowfullscreen="true"></iframe></div>
      <div class="v-label"><p>Bilibili: <strong>Wwise</strong> - 优化频段的侧链压缩</p></div>
    </div>
    <div class="swiper-slide">
      <div class="v-container"><iframe src="//player.bilibili.com/player.html?bvid=BV1mx4y1S7JJ&high_quality=1&danmaku=0" scrolling="no" frameborder="no" allowfullscreen="true"></iframe></div>
      <div class="v-label"><p>Bilibili: <strong>Spatial Audio</strong> - 声障, 声笼, 衍射与透射</p></div>
    </div>
    <div class="swiper-slide">
      <div class="v-container"><iframe src="//player.bilibili.com/player.html?bvid=BV1mu4m1g7ic&high_quality=1&danmaku=0" scrolling="no" frameborder="no" allowfullscreen="true"></iframe></div>
      <div class="v-label"><p>Bilibili: <strong>Spatial Audio</strong> - 房间混响与 Portal</p></div>
    </div>
    <div class="swiper-slide">
      <div class="v-container"><iframe src="//player.bilibili.com/player.html?bvid=BV1dM4y1h7AA&high_quality=1&danmaku=0" scrolling="no" frameborder="no" allowfullscreen="true"></iframe></div>
      <div class="v-label"><p>Bilibili: <strong>UE5 + Wwise</strong> - 识别地板材质切换脚步声</p></div>
    </div>
  </div>
  <div class="swiper-button-next"></div><div class="swiper-button-prev"></div><div class="swiper-pagination"></div>
</div>

<script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
<script>
  var swiper = new Swiper(".mySwiper", {
    slidesPerView: 1.2, centeredSlides: true, spaceBetween: 20, loop: true,
    pagination: { el: ".swiper-pagination", clickable: true },
    navigation: { nextEl: ".swiper-button-next", prevEl: ".swiper-button-prev" },
    breakpoints: { 768: { slidesPerView: 1.5 } }
  });
</script>
