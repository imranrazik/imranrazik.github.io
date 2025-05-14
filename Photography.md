---
layout: grid
---
# Photography
---

<div class="row"> 
  <div class="column">
    <img src="/assets/photos/chiroptology/01_IMG_2563.jpg" loading="lazy" decoding="async" style="width:100%" alt="01">
    <img src="/assets/photos/chiroptology/02_IMG_2547.JPG" loading="lazy" decoding="async" style="width:100%" alt="02">
    <img src="/assets/photos/chiroptology/03_IMG_5306.JPG" loading="lazy" decoding="async" style="width:100%" alt="03">
    <img src="/assets/photos/chiroptology/04_IMG_2406.JPG" loading="lazy" decoding="async" style="width:100%" alt="04">
    <img src="/assets/photos/chiroptology/05_IMG_1995.JPG" loading="lazy" decoding="async" style="width:100%" alt="05">
  </div>
  <div class="column">
    <img src="/assets/photos/chiroptology/06_P1012854.JPG" loading="lazy" decoding="async" style="width:100%" alt="06">
    <img src="/assets/photos/chiroptology/07_P1012904.JPG" loading="lazy" decoding="async" style="width:100%" alt="07">
    <img src="/assets/photos/chiroptology/08_37499008_Unknown.JPG" loading="lazy" decoding="async" style="width:100%" alt="08">
    <img src="/assets/photos/chiroptology/09_IMG_1747.JPG" loading="lazy" decoding="async" style="width:100%" alt="09">
    <img src="/assets/photos/chiroptology/10_IMG_3159.JPG" loading="lazy" decoding="async" style="width:100%" alt="10">
  </div>  
  <div class="column">
    <img src="/assets/photos/chiroptology/11_IMG_5163.JPG" loading="lazy" decoding="async" style="width:100%" alt="11">
    <img src="/assets/photos/chiroptology/12_IMG_0363.JPG" loading="lazy" decoding="async" style="width:100%" alt="12">
    <img src="/assets/photos/chiroptology/13_IMG_2666.JPG" loading="lazy" decoding="async" style="width:100%" alt="13">
    <img src="/assets/photos/chiroptology/14_IMG_1759.JPG" loading="lazy" decoding="async" style="width:100%" alt="14">
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
  const images = Array.from(document.querySelectorAll(".row img"));
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
    modal.style.display = "block";
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

  // Optional: close when clicking outside image
  modal.addEventListener("click", function (e) {
    if (e.target === modal) closeModal();
  });
</script>


<style>
/* Modal styling */
.modal {
  position: fixed;
  z-index: 1;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.8);  /* Black background with opacity */
  display: flex;
  justify-content: center;
  align-items: center;
}

.modal-content {
  max-width: 60%;
  max-height: 60%;
  margin: auto;
}

.close {
  position: absolute;
  top: 15px;
  right: 35px;
  color: #f1f1f1;
  font-size: 40px;
  font-weight: bold;
  cursor: pointer;
  background-color: transparent;
  border: none;
}

.close:hover,
.close:focus {
  color: #bbb;
  text-decoration: none;
  cursor: pointer;
}

a.prev, a.next {
  position: absolute;
  top: 50%;
  color: white;
  font-size: 40px;
  font-weight: bold;
  cursor: pointer;
  padding: 16px;
  border: none;
}

a.prev {
  left: 10px;
}

a.next {
  right: 10px;
}

a.prev:hover, a.next:hover {
  color: #bbb;
}

a.prev, a.next {
  font-size: 24px; /* Make arrows smaller */
  color: white; /* Keep them white */
  text-decoration: none; /* Remove any underlining */
}

a.prev:hover, a.next:hover {
  color: #bbb; /* Change color slightly on hover */
}
</style>
