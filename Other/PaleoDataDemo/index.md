---
layout: page
title: What incomplete data hides
subtitle: An interactive demonstration of how proxy bias, noise, resolution and coverage limit paleoclimate reconstructions
full-width: true
---

[Open the demo in its own window](/Other/PaleoDataDemo/app.html){:target="_blank"}

<iframe id="demo-frame"
  src="/Other/PaleoDataDemo/app.html"
  title="What incomplete data hides"
  style="width:100%; height:1500px; border:1px solid #ccc; border-radius:6px;"
  loading="lazy"></iframe>

<script>
  // fit the frame height to the demo's content (same website, so this is allowed)
  (function () {
    var f = document.getElementById('demo-frame');
    function fit() {
      try { f.style.height = (f.contentDocument.documentElement.scrollHeight + 20) + 'px'; } catch (e) {}
    }
    f.addEventListener('load', function () {
      fit();
      try { new ResizeObserver(fit).observe(f.contentDocument.body); } catch (e) {}
    });
  })();
</script>
