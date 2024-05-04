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
        <img src="/assets/illustrations/page1.jpg" loading="lazy" decoding="async" alt="01">
    </div>
  </div>
  
  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/page2.jpg" loading="lazy" decoding="async" alt="02">
    </div>
  </div>
  
  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/vampire_poster.png" loading="lazy" decoding="async" alt="03">
    </div>
  </div>
  
  <div class="responsive">
    <div class="gallery">
        <img src="/assets/illustrations/trachops_poster.png" loading="lazy" decoding="async" alt="04">
    </div>
  </div>
</div>

<table align="center" style="width:100%">
    <tr>
        <td align="center" width ="25%"><img src="/assets/illustrations/vampire_v02.png" width="100%"></td>
        <td align="center" width ="25%"><img src="/assets/illustrations/blue naped chlorophonia.png" width="100%"></td>
        <td align="center" width ="25%"><img src="/assets/illustrations/trachops.png" width="100%"></td>  
        <td align="center" width ="25%"><img src="/assets/illustrations/tungara.png" width="90%"></td>
    </tr>
    <tr>
        <td align="center" width ="25%"><img src="/assets/illustrations/glass frog.png" width="100%"></td>
        <td align="center" width ="25%"><img src="/assets/illustrations/aracari.png" width="100%"></td>
        <td align="center" width ="25%"><img src="/assets/illustrations/jacobin.png" width="100%"></td>  
        <td align="center" width ="25%"><img src="/assets/illustrations/flowerpiercer.png" width="90%"></td>
    </tr>
    <tr>
        <td align="center"><img src="/assets/illustrations/ectophylla.png" width="100%"></td>
        <td align="center"><img src="/assets/illustrations/phyllostomus.png" width="100%"></td>
        <td align="center"><img src="/assets/illustrations/noctilio_v02.png" width="100%"></td>
        <td align="center"><img src="/assets/illustrations/lonch2.png" width="100%"></td>
    </tr>
    <tr>
        <td align="center"><img src="/assets/illustrations/pronghorn.png" width="80%"></td>
        <td align="center"><img src="/assets/illustrations/anteater.png" width="100%"></td>
        <td align="center"><img src="/assets/illustrations/molossus_03.png" width="100%"></td>
        <td align="center"><img src="/assets/illustrations/saccopteryxoffset.png" width="100%"></td>
    </tr>
    <tr>
        <td align="center"><img src="/assets/illustrations/micronycterisoffset.png" width="100%"></td>
        <td align="center"><img src="/assets/illustrations/molossus_02.png" width="100%"></td>
        <td align="center"><img src="/assets/illustrations/spixoffset.png" width="100%"></td>
        <td align="center"><img src="/assets/illustrations/centurio.png" width="100%"></td>
    </tr>
    <tr>
        <td align="center"><img src="/assets/illustrations/santa marta antbird.png" width="100%"></td>
        <td align="center"><img src="/assets/illustrations/emeraldbird.png" width="100%"></td>
        <td align="center"><img src="/assets/illustrations/cat.png" width="100%"></td>
        <td align="center"><img src="/assets/illustrations/motmot.png" width="100%"></td>
    </tr>
    <tr>
        <td align="center"><img src="/assets/illustrations/lonchorhina.png" width="100%"></td>
        <td align="center"><img src="/assets/illustrations/glossophagaoffset.png" width="100%"></td>
        <td align="center"><img src="/assets/illustrations/cow_v02_color_offset.png" width="100%"></td>
        <td align="center"><img src="/assets/illustrations/redeye.png" width="100%"></td>
    </tr>
    <tr>
        <td align="center"><img src="/assets/illustrations/tinamou.png" width="100%"></td>
        <td align="center"><img src="/assets/illustrations/coati.png" width="75%"></td>
        <td align="center"><img src="/assets/illustrations/wellington.png" width="100%"></td>
        <td align="center"><img src="/assets/illustrations/vampire_v03.png" width="100%"></td>
    </tr>
    <tr>
        <td align="center"><img src="/assets/illustrations/hila.png" width="100%"></td>
        <td align="center"><img src="/assets/illustrations/ajoffset.png" width="100%"></td>
        <td align="center"><img src="/assets/illustrations/anole.png" width="100%"></td>
        <td align="center"><img src="/assets/illustrations/katydid.png" width="100%"></td>
    </tr>
</table> <br/>

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



