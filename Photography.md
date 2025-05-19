---
layout: grid
---
# Photography
---

<div class="grid"> 
  <div class="gallery">
    <img src="/assets/photos/chiroptology/01_IMG_2563.jpg" loading="lazy" decoding="async" style="width:100%" alt="01">
  </div>
  <div class="gallery">
    <img src="/assets/photos/chiroptology/02_IMG_2547.JPG" loading="lazy" decoding="async" style="width:100%" alt="02">
  </div>
  <div class="gallery">
    <img src="/assets/photos/chiroptology/03_IMG_5306.JPG" loading="lazy" decoding="async" style="width:100%" alt="03">
  </div>
  <div class="gallery">
    <img src="/assets/photos/chiroptology/04_IMG_2406.JPG" loading="lazy" decoding="async" style="width:100%" alt="04">
  </div>
  <div class="gallery">
    <img src="/assets/photos/chiroptology/05_IMG_1995.JPG" loading="lazy" decoding="async" style="width:100%" alt="05">
  </div>
  <div class="gallery">
    <img src="/assets/photos/chiroptology/06_P1012854.JPG" loading="lazy" decoding="async" style="width:100%" alt="06">
  </div>
  <div class="gallery">
    <img src="/assets/photos/chiroptology/07_P1012904.JPG" loading="lazy" decoding="async" style="width:100%" alt="07">
  </div>
  <div class="gallery">
    <img src="/assets/photos/chiroptology/08_37499008_Unknown.JPG" loading="lazy" decoding="async" style="width:100%" alt="08">
  </div>
  <div class="gallery">
    <img src="/assets/photos/chiroptology/09_IMG_1747.JPG" loading="lazy" decoding="async" style="width:100%" alt="09">
  </div> 
  <div class="gallery">
    <img src="/assets/photos/chiroptology/10_IMG_3159.JPG" loading="lazy" decoding="async" style="width:100%" alt="10">
  </div>
  <div class="gallery">
    <img src="/assets/photos/chiroptology/11_IMG_5163.JPG" loading="lazy" decoding="async" style="width:100%" alt="11">
  </div>
  <div class="gallery">
    <img src="/assets/photos/chiroptology/12_IMG_0363.JPG" loading="lazy" decoding="async" style="width:100%" alt="12">
  </div>
  <div class="gallery">
    <img src="/assets/photos/chiroptology/13_IMG_2666.JPG" loading="lazy" decoding="async" style="width:100%" alt="13">
  </div>
  <div class="gallery">
    <img src="/assets/photos/chiroptology/14_IMG_1759.JPG" loading="lazy" decoding="async" style="width:100%" alt="14">
  </div>
  <div class="gallery">
    <img src="/assets/photos/chiroptology/15_IMG_5222.JPG" loading="lazy" decoding="async" style="width:100%" alt="15">
  </div>
</div>
<br>

<!-- Modal -->
  <div id="modal" class="modal">
    <span class="close" onclick="closeModal()">&times;</span>
    <div class="modal-content">
      <img id="modal-image" src="" alt="">
      <a class="prev" onclick="changeSlide(-1)">&#10094;</a>
      <a class="next" onclick="changeSlide(1)">&#10095;</a>
    </div>
  </div>

  <script>
    const images = Array.from(document.querySelectorAll(".gallery img"));
    const modal = document.getElementById("modal");
    const modalImage = document.getElementById("modal-image");
    let currentIndex = 0;

    images.forEach((img, index) => {
      img.addEventListener("click", () => {
        currentIndex = index;
        openModal();
      });
    });

    function openModal() {
      modal.style.display = "flex";
      showSlide(currentIndex);
    }

    function closeModal() {
      modal.style.display = "none";
    }

    function changeSlide(n) {
      currentIndex = (currentIndex + n + images.length) % images.length;
      showSlide(currentIndex);
    }

    function showSlide(index) {
      modalImage.src = images[index].src;
      modalImage.alt = images[index].alt;
    }

    modal.addEventListener("click", function (e) {
      if (!e.target.closest(".modal-content")) {
        closeModal();
      }
    });

    modalImage.addEventListener("click", function (e) {
      e.stopPropagation();
    });

    document.addEventListener("keydown", function (e) {
      if (modal.style.display === "flex") {
        if (e.key === "ArrowLeft") {
          changeSlide(-1);
        } else if (e.key === "ArrowRight") {
          changeSlide(1);
        } else if (e.key === "Escape") {
          closeModal();
        }
      }
    });
  </script>
