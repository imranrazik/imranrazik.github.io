---
layout: grid
---
# Photography
---

<div class="row"> 
  <div class="column">
    <img src="/assets/photos/chiroptology/01_IMG_2563.jpg" loading="lazy" decoding="async" style="width:100%" alt="01" onclick="openModal();currentSlide(1)">
    <img src="/assets/photos/chiroptology/02_IMG_2547.JPG" loading="lazy" decoding="async" style="width:100%" alt="02" onclick="openModal();currentSlide(2)">
    <img src="/assets/photos/chiroptology/03_IMG_5306.JPG" loading="lazy" decoding="async" style="width:100%" alt="03" onclick="openModal();currentSlide(3)">
    <img src="/assets/photos/chiroptology/04_IMG_2406.JPG" loading="lazy" decoding="async" style="width:100%" alt="04" onclick="openModal();currentSlide(4)">
    <img src="/assets/photos/chiroptology/05_IMG_1995.JPG" loading="lazy" decoding="async" style="width:100%" alt="05" onclick="openModal();currentSlide(5)">
  </div>
  <div class="column">
    <img src="/assets/photos/chiroptology/06_P1012854.JPG" loading="lazy" decoding="async" style="width:100%" alt="06" onclick="openModal();currentSlide(6)">
    <img src="/assets/photos/chiroptology/07_P1012904.JPG" loading="lazy" decoding="async" style="width:100%" alt="07" onclick="openModal();currentSlide(7)">
    <img src="/assets/photos/chiroptology/08_37499008_Unknown.JPG" loading="lazy" decoding="async" style="width:100%" alt="08" onclick="openModal();currentSlide(8)">
    <img src="/assets/photos/chiroptology/09_IMG_1747.JPG" loading="lazy" decoding="async" style="width:100%" alt="09" onclick="openModal();currentSlide(9)">
    <img src="/assets/photos/chiroptology/10_IMG_3159.JPG" loading="lazy" decoding="async" style="width:100%" alt="10" onclick="openModal();currentSlide(10)">
  </div>  
  <div class="column">
    <img src="/assets/photos/chiroptology/11_IMG_5163.JPG" loading="lazy" decoding="async" style="width:100%" alt="11" onclick="openModal();currentSlide(11)">
    <img src="/assets/photos/chiroptology/12_IMG_0363.JPG" loading="lazy" decoding="async" style="width:100%" alt="12" onclick="openModal();currentSlide(12)">
    <img src="/assets/photos/chiroptology/13_IMG_2666.JPG" loading="lazy" decoding="async" style="width:100%" alt="13" onclick="openModal();currentSlide(13)">
    <img src="/assets/photos/chiroptology/14_IMG_1759.JPG" loading="lazy" decoding="async" style="width:100%" alt="14" onclick="openModal();currentSlide(14)">
    <img src="/assets/photos/chiroptology/15_IMG_5222.JPG" loading="lazy" decoding="async" style="width:100%" alt="15" onclick="openModal();currentSlide(15)">
  </div>
</div>
<br>
<div id="gallery-container">
  <div class="responsive">
    <div class="gallery">
      <a href="https://drive.google.com/file/d/10nz_KLOAVNlXMGAMwH5BJrA3bTe4ufYt/view?usp=sharing" target="_blank">
        <img src="/assets/illustrations/page1.jpg" loading="lazy" decoding="async">
      </a>
    </div>
  </div>
  
  <div class="responsive">
    <div class="gallery">
      <a href="https://drive.google.com/file/d/10nvEE8OEBtulAauLNFdgTiL9u4FC4FGO/view?usp=sharing" target="_blank">
        <img src="/assets/illustrations/page2.jpg" loading="lazy" decoding="async">
      </a>
    </div>
  </div>

<!-- Modal -->
<div id="myModal" class="modal">
  <span class="close" onclick="closeModal()">&times;</span>
  <div class="modal-content">
    <!-- Slides (15) -->
    <div class="mySlides"><img src="/assets/photos/chiroptology/01_IMG_2563.jpg" alt="01" /></div>
    <div class="mySlides"><img src="/assets/photos/chiroptology/02_IMG_2547.JPG" alt="02" /></div>
    <div class="mySlides"><img src="/assets/photos/chiroptology/03_IMG_5306.JPG" alt="03" /></div>
    <div class="mySlides"><img src="/assets/photos/chiroptology/04_IMG_2406.JPG" alt="04" /></div>
    <div class="mySlides"><img src="/assets/photos/chiroptology/05_IMG_1995.JPG" alt="05" /></div>
    <div class="mySlides"><img src="/assets/photos/chiroptology/06_P1012854.JPG" alt="06" /></div>
    <div class="mySlides"><img src="/assets/photos/chiroptology/07_P1012904.JPG" alt="07" /></div>
    <div class="mySlides"><img src="/assets/photos/chiroptology/08_37499008_Unknown.JPG" alt="08" /></div>
    <div class="mySlides"><img src="/assets/photos/chiroptology/09_IMG_1747.JPG" alt="09" /></div>
    <div class="mySlides"><img src="/assets/photos/chiroptology/10_IMG_3159.JPG" alt="10" /></div>
    <div class="mySlides"><img src="/assets/photos/chiroptology/11_IMG_5163.JPG" alt="11" /></div>
    <div class="mySlides"><img src="/assets/photos/chiroptology/12_IMG_0363.JPG" alt="12" /></div>
    <div class="mySlides"><img src="/assets/photos/chiroptology/13_IMG_2666.JPG" alt="13" /></div>
    <div class="mySlides"><img src="/assets/photos/chiroptology/14_IMG_1759.JPG" alt="14" /></div>
    <div class="mySlides"><img src="/assets/photos/chiroptology/15_IMG_5222.JPG" alt="15" /></div>

    <!-- Navigation -->
    <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
    <a class="next" onclick="plusSlides(1)">&#10095;</a>

    <div class="caption-container">
      <p id="caption"></p>
    </div>
  </div>
</div>

<script>
  let modal, slides, slideIndex;

modal = document.getElementById("myModal");
slides = document.getElementsByClassName("mySlides");
slideIndex = 1;

function openModal() {
  modal.style.display = "block";
  showSlides(slideIndex);
}

function closeModal() {
  modal.style.display = "none";
}

function plusSlides(n) {
  showSlides(slideIndex += n);
}

function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  if (n > slides.length) slideIndex = 1;
  if (n < 1) slideIndex = slides.length;
  for (let i = 0; i < slides.length; i++) {
    slides[i].style.display = "none";
  }
  slides[slideIndex - 1].style.display = "block";
}

document.addEventListener("DOMContentLoaded", function () {
  // Close on outside click
  modal.addEventListener('click', function (e) {
    if (e.target === modal) closeModal();
  });

});

</script>
