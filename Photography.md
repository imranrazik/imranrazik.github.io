---
layout: grid
---
# Photography
---

<div class="row"> 
  <div class="column">
    <img src="/assets/photos/chiroptology/01_IMG_2563.jpg" loading="lazy" decoding="async" style="width:100%" alt="01" onclick="openModal(this)">
    <img src="/assets/photos/chiroptology/02_IMG_2547.JPG" loading="lazy" decoding="async" style="width:100%" alt="02" onclick="openModal(this)">
    <img src="/assets/photos/chiroptology/03_IMG_5306.JPG" loading="lazy" decoding="async" style="width:100%" alt="03" onclick="openModal(this)">
    <img src="/assets/photos/chiroptology/04_IMG_2406.JPG" loading="lazy" decoding="async" style="width:100%" alt="04" onclick="openModal(this)">
    <img src="/assets/photos/chiroptology/05_IMG_1995.JPG" loading="lazy" decoding="async" style="width:100%" alt="05" onclick="openModal(this)">
  </div>
  <div class="column">
    <img src="/assets/photos/chiroptology/06_P1012854.JPG" loading="lazy" decoding="async" style="width:100%" alt="06" onclick="openModal(this)">
    <img src="/assets/photos/chiroptology/07_P1012904.JPG" loading="lazy" decoding="async" style="width:100%" alt="07" onclick="openModal(this)">
    <img src="/assets/photos/chiroptology/08_37499008_Unknown.JPG" loading="lazy" decoding="async" style="width:100%" alt="08" onclick="openModal(this)">
    <img src="/assets/photos/chiroptology/09_IMG_1747.JPG" loading="lazy" decoding="async" style="width:100%" alt="09" onclick="openModal(this)">
    <img src="/assets/photos/chiroptology/10_IMG_3159.JPG" loading="lazy" decoding="async" style="width:100%" alt="10" onclick="openModal(this)">
  </div>  
  <div class="column">
    <img src="/assets/photos/chiroptology/11_IMG_5163.JPG" loading="lazy" decoding="async" style="width:100%" alt="11" onclick="openModal(this)">
    <img src="/assets/photos/chiroptology/12_IMG_0363.JPG" loading="lazy" decoding="async" style="width:100%" alt="12" onclick="openModal(this)">
    <img src="/assets/photos/chiroptology/13_IMG_2666.JPG" loading="lazy" decoding="async" style="width:100%" alt="13" onclick="openModal(this)">
    <img src="/assets/photos/chiroptology/14_IMG_1759.JPG" loading="lazy" decoding="async" style="width:100%" alt="14" onclick="openModal(this)">
    <img src="/assets/photos/chiroptology/15_IMG_5222.JPG" loading="lazy" decoding="async" style="width:100%" alt="15" onclick="openModal(this)">
  </div>
</div>
<br>

<!-- Modal -->
<div id="myModal" class="modal" style="display:none;">
  <span class="close" onclick="closeModal()">&times;</span>
  <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
  <img class="modal-content" id="modal-img">
  <div id="caption"></div>
  <a class="next" onclick="plusSlides(1)">&#10095;</a>
</div>

<script>
// Variables to manage the modal and slides
let modal, modalImg, caption, slideIndex;

modal = document.getElementById("myModal");
modalImg = document.getElementById("modal-img");
caption = document.getElementById("caption");
slideIndex = 1;

// Open modal and show the clicked image
function openModal(img) {
  modal.style.display = "block";
  modalImg.src = img.src;  // Set the clicked image as the modal image
  caption.innerHTML = img.alt;  // Optionally, show the alt text as caption
  slideIndex = Array.from(img.parentElement.children).indexOf(img) + 1;
}

// Close the modal
function closeModal() {
  modal.style.display = "none";
}

// Navigate to the next or previous image
function plusSlides(n) {
  slideIndex += n;
  showSlides(slideIndex);
}

// Set the current slide
function showSlides(n) {
  const allImages = document.querySelectorAll('.column img');
  if (n > allImages.length) slideIndex = 1;
  if (n < 1) slideIndex = allImages.length;

  const currentImage = allImages[slideIndex - 1];
  modalImg.src = currentImage.src;
  caption.innerHTML = currentImage.alt;
}

// Close modal if clicked outside the image
window.onclick = function(event) {
  if (event.target === modal) {
    closeModal();
  }
}
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
  background-color: rgba(0,0,0,0.8);  /* Black background with opacity */
  display: none;
  align-items: center;
  justify-content: center;
}

.modal-content {
  max-width: 80%;
  max-height: 80%;
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
  font-size: 24px;
  font-weight: bold;
  cursor: pointer;
  padding: 16px;
  background-color: rgba(0, 0, 0, 0.5);
  border: none;
  border-radius: 50%;
  user-select: none;
}

a.prev {
  left: 10px;
}

a.next {
  right: 10px;
}

a.prev:hover, a.next:hover {
  background-color: rgba(0, 0, 0, 0.7);
}
</style>
