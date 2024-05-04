---
layout: default
---
# Design
---

My work displayed below is licensed under a [CC BY-NC-SA 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/). <br/>

<div id="loading" class="loading">
  <div class="loader-container">
    <div class="dot-pulse"></div>
  </div>
</div>

<div id="gallery-container" style="display: none;">
  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/vampire_v02.png" loading="lazy" decoding="async" alt="01">
    </div>
  </div>
  
  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/tungara.png" loading="lazy" decoding="async" alt="02">
    </div>
  </div>
  
  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/aracari.png" loading="lazy" decoding="async" alt="03">
    </div>
  </div>
  
  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/glass frog.png" loading="lazy" decoding="async" alt="04">
    </div>
  </div>

  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/jacobin.png" loading="lazy" decoding="async" alt="04">
    </div>
  </div>

  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/ectophylla.png" loading="lazy" decoding="async" alt="04">
    </div>
  </div>

  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/noctilio_v02.png" loading="lazy" decoding="async" alt="04">
    </div>
  </div>

  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/lonch2.png" loading="lazy" decoding="async" alt="04">
    </div>
  </div>

  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/noctilio_v02.png" loading="lazy" decoding="async" alt="04">
    </div>
  </div>

  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/pronghorn.png" loading="lazy" decoding="async" alt="04">
    </div>
  </div>

  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/anteater.png" loading="lazy" decoding="async" alt="04">
    </div>
  </div>

  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/molossus_03.png" loading="lazy" decoding="async" alt="04">
    </div>
  </div>

  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/pronghorn.png" loading="lazy" decoding="async" alt="04">
    </div>
  </div>

  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/molossus_02.png" loading="lazy" decoding="async" alt="04">
    </div>
  </div>

  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/pronghorn.png" loading="lazy" decoding="async" alt="04">
    </div>
  </div>

  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/motmot.png" loading="lazy" decoding="async" alt="04">
    </div>
  </div>

  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/cat.png" loading="lazy" decoding="async" alt="04">
    </div>
  </div>

  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/tinamou.png" loading="lazy" decoding="async" alt="04">
    </div>
  </div>

  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/wellington.png" loading="lazy" decoding="async" alt="04">
    </div>
  </div>

  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/hila.png" loading="lazy" decoding="async" alt="04">
    </div>
  </div>

  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/emeraldbird.png" loading="lazy" decoding="async" alt="04">
    </div>
  </div>
</div>

<script>
document.addEventListener("DOMContentLoaded", function() {
    // Hide the gallery initially
    document.getElementById("gallery-container").style.display = "none";

    // Display loading symbol
    document.getElementById("loading").style.display = "block";

    // Check if all images are loaded
    var images = document.getElementById("gallery-container").getElementsByTagName("img");
    var loadedCount = 0;

    for (var i = 0; i < images.length; i++) {
        images[i].addEventListener("load", function() {
            loadedCount++;
            if (loadedCount === images.length) {
                // All images loaded, hide loading symbol and show gallery
                document.getElementById("loading").style.display = "none";
                document.getElementById("gallery-container").style.display = "block";
            }
        });
    }
});
</script>



