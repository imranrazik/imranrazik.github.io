---
layout: default
---

<div class="slideshow-container">

<div class="mySlides fade">
  <img src="/assets/photos/chiroptology/01_IMG_2563.jpg" style="height=auto" style="width:100%">
</div>

<div class="mySlides fade">
  <img src="/assets/photos/chiroptology/02_IMG_2547.JPG" style="height=auto" style="width:100%">
</div>

<div class="mySlides fade">
  <img src="/assets/photos/chiroptology/03_IMG_5306.JPG" style="height=auto" style="width:100%">
</div>

<div class="mySlides fade">
  <img src="/assets/photos/chiroptology/04_IMG_2406.JPG" style="height=auto" style="width:100%">
</div>

<div class="mySlides fade">
  <img src="/assets/photos/chiroptology/05_IMG_1995.JPG" style="height=auto" style="width:100%">
</div>

<div class="mySlides fade">
  <img src="/assets/photos/chiroptology/06_P1012854.JPG" style="height=auto" style="width:100%">
</div>

<div class="mySlides fade">
  <img src="/assets/photos/chiroptology/07_P1012904.JPG" style="height=auto" style="width:100%">
</div>

<div class="mySlides fade">
  <img src="/assets/photos/chiroptology/08_37499008_Unknown.JPG" style="height=auto" style="width:100%">
</div>

<div class="mySlides fade">
  <img src="/assets/photos/chiroptology/09_IMG_1747.JPG" style="height=auto" style="width:100%">
</div>

<div class="mySlides fade">
  <img src="/assets/photos/chiroptology/10_IMG_3159.JPG" style="height=auto" style="width:100%">
</div>

<div class="mySlides fade">
  <img src="/assets/photos/chiroptology/11_IMG_5163.JPG" style="height=auto" style="width:100%">
</div>

<div class="mySlides fade">
  <img src="/assets/photos/chiroptology/12_IMG_0363.JPG" style="height=auto" style="width:100%">
</div>

<div class="mySlides fade">
  <img src="/assets/photos/chiroptology/13_IMG_2666.JPG" style="height=auto" style="width:100%">
</div>

<div class="mySlides fade">
  <img src="/assets/photos/chiroptology/14_IMG_1759.JPG" style="height=auto" style="width:100%">
</div>

<div class="mySlides fade">
  <img src="/assets/photos/chiroptology/15_IMG_5222.JPG" style="height=auto" style="width:100%">
</div>

<a class="prev" onclick="plusSlides(-1)">❮</a>
<a class="next" onclick="plusSlides(1)">❯</a>

</div>
<br>

<script>
let slideIndex = 1;
showSlides(slideIndex);

function plusSlides(n) {
  showSlides(slideIndex += n);
}

function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  let i;
  let slides = document.getElementsByClassName("mySlides");
  let dots = document.getElementsByClassName("dot");
  if (n > slides.length) {slideIndex = 1}    
  if (n < 1) {slideIndex = slides.length}
  for (i = 0; i < slides.length; i++) {
    slides[i].style.display = "none";  
  }
  for (i = 0; i < dots.length; i++) {
    dots[i].className = dots[i].className.replace(" active", "");
  }
  slides[slideIndex-1].style.display = "block";  
  dots[slideIndex-1].className += " active";
}
</script>
