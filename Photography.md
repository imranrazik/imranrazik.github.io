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
  
  <!-- Arrows go here -->
  <a class="prev" onclick="changeSlide(-1)">&#10094;</a>
  <a class="next" onclick="changeSlide(1)">&#10095;</a>

  <!-- Only image inside modal-content -->
  <div class="modal-content">
    <img id="modal-image" src="" alt="">
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

// Close modal when clicking outside of the image area (on the background)
modal.addEventListener("click", function (e) {
  // Only close the modal if the click is outside the modal-content
  if (!e.target.closest(".modal-content")) {
    closeModal();
  }
});

// Prevent clicks on the image from closing the modal (we only want clicks on the background)
modalImage.addEventListener("click", function (e) {
  e.stopPropagation();  // Prevent click from propagating to the modal (background)
});

// Keyboard controls: Arrow keys to navigate and ESC to close
document.addEventListener("keydown", function (e) {
  if (modal.style.display === "flex") {
    if (e.key === "ArrowLeft") {
      changeSlide(-1); // Move to previous image
    } else if (e.key === "ArrowRight") {
      changeSlide(1); // Move to next image
    } else if (e.key === "Escape") {
      closeModal(); // Close the modal
    }
  }
});
</script>


<style>
/* Modal styling */
.modal {
  display: none;
  position: fixed;
  z-index: 1;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.8);
  justify-content: center;
  align-items: center;
}

.modal-content {
  position: relative;
  z-index: 2;
  max-width: 90vw;
  max-height: 90vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

.modal-content img {
  max-width: 70%;
  max-height: 70%;
  display: block;
}

a.prev, a.next {
  position: fixed; /* fixed instead of absolute */
  top: 50%;
  transform: translateY(-50%);
  font-size: 24px;
  font-weight: bold;
  color: white;
  background-color: transparent;
  padding: 16px;
  z-index: 2;
  cursor: pointer;
  text-decoration: none;
}

a.prev {
  left: 20px;
}

a.next {
  right: 20px;
}

a.prev:hover, a.next:hover {
  color: #bbb;
}
</style>
