---
layout: cv
permalink: /cv/
title: CV
nav: true
nav_order: 5
cv_format: rendercv # options: rendercv, jsonresume
toc:
  sidebar: left
---

<style>
  .table-cv td {
    vertical-align: middle;
  }
</style>

<script>
  // The theme's default tocbot offset (80px) is tuned for the fixed navbar
  // alone; on this page the extra card spacing between CV sections pushes
  // each heading a bit further down, so the sidebar highlight lags one
  // section behind while scrolling. Re-init with a larger offset once the
  // page (and the theme's own tocbot.init call) has finished loading.
  window.addEventListener("load", function () {
    if (window.tocbot && typeof window.tocbot.init === "function") {
      window.tocbot.destroy();
      window.tocbot.init({
        tocSelector: "#toc-sidebar",
        contentSelector: '[role="main"]',
        headingSelector: "h2, h3",
        ignoreSelector: "[data-toc-skip]",
        hasInnerContainers: true,
        collapseDepth: 6,
        orderedList: false,
        activeLinkClass: "is-active-link",
        scrollSmooth: true,
        scrollSmoothOffset: -100,
        headingsOffset: 100,
      });
    }
  });
</script>
