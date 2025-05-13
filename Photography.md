---
layout: grid
---
# Photography
---

<div class="row"> 
  <div class="column">
    <img src="/assets/photos/chiroptology/01_IMG_2563.jpg" loading="lazy" decoding="async" style="width:100%" alt="01"
  onclick="openModal();currentSlide(1)">
    <img src="/assets/photos/chiroptology/02_IMG_2547.JPG" loading="lazy" decoding="async" alt="02"
  onclick="openModal();currentSlide(2)">
    <img src="/assets/photos/chiroptology/03_IMG_5306.JPG" loading="lazy" decoding="async" alt="03"
  onclick="openModal();currentSlide(3)">
    <img src="/assets/photos/chiroptology/04_IMG_2406.JPG" loading="lazy" decoding="async" alt="04"
  onclick="openModal();currentSlide(4)">
    <img src="/assets/photos/chiroptology/05_IMG_1995.JPG" loading="lazy" decoding="async" alt="05"
  onclick="openModal();currentSlide(5)">
  </div>
  <div class="column">
    <img src="/assets/photos/chiroptology/06_P1012854.JPG" loading="lazy" decoding="async" alt="06"
  onclick="openModal();currentSlide(6)">
    <img src="/assets/photos/chiroptology/07_P1012904.JPG" loading="lazy" decoding="async" alt="07"
  onclick="openModal();currentSlide(7)">
    <img src="/assets/photos/chiroptology/08_37499008_Unknown.JPG" loading="lazy" decoding="async" alt="08"
  onclick="openModal();currentSlide(8)">
    <img src="/assets/photos/chiroptology/09_IMG_1747.JPG" loading="lazy" decoding="async" alt="09"
  onclick="openModal();currentSlide(9)">
    <img src="/assets/photos/chiroptology/10_IMG_3159.JPG" loading="lazy" decoding="async" alt="10"
  onclick="openModal();currentSlide(10)">
  </div>  
  <div class="column">
    <img src="/assets/photos/chiroptology/11_IMG_5163.JPG" loading="lazy" decoding="async" alt="11"
  onclick="openModal();currentSlide(11)">
    <img src="/assets/photos/chiroptology/12_IMG_0363.JPG" loading="lazy" decoding="async" alt="12"
  onclick="openModal();currentSlide(12)">
    <img src="/assets/photos/chiroptology/13_IMG_2666.JPG" loading="lazy" decoding="async" alt="13"
  onclick="openModal();currentSlide(13)">
    <img src="/assets/photos/chiroptology/14_IMG_1759.JPG" loading="lazy" decoding="async" alt="14"
  onclick="openModal();currentSlide(14)">
    <img src="/assets/photos/chiroptology/15_IMG_5222.JPG" loading="lazy" decoding="async" alt="15"
  onclick="openModal();currentSlide(15)">
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

  <div id="myModal" class="modal">
    <span class="close cursor" onclick="closeModal()">&times;</span>
    <div class="modal-content">
  
      <div class="mySlides">
        <img src="/assets/photos/chiroptology/01_IMG_2563.jpg" style="height:auto; width:99%">
      </div>
  
      <div class="mySlides">
        <img src="/assets/photos/chiroptology/02_IMG_2547.JPG" style="height:auto; width:99%">
      </div>
  
      <div class="mySlides">
        <img src="/assets/photos/chiroptology/03_IMG_5306.JPG" style="height:auto; width:99%">
      </div>
      
      <div class="mySlides">
        <img src="/assets/photos/chiroptology/04_IMG_2406.JPG" style="height:auto; width:99%">   
      </div>
        
      <div class="mySlides">
        <img src="/assets/photos/chiroptology/05_IMG_1995.JPG" style="height:auto; width:99%">   
      </div>
  
      <div class="mySlides">
        <img src="/assets/photos/chiroptology/06_P1012854.JPG" style="height:auto; width:99%">   
      </div>
  
      <div class="mySlides">
        <img src="/assets/photos/chiroptology/07_P1012904.JPG" style="height:auto; width:99%">   
      </div>
  
      <div class="mySlides">
        <img src="/assets/photos/chiroptology/08_37499008_Unknown.JPG" style="height:auto; width:99%">   
      </div>
  
      <div class="mySlides">
        <img src="/assets/photos/chiroptology/09_IMG_1747.JPG" style="height:auto; width:99%">   
      </div>
  
      <div class="mySlides">
        <img src="/assets/photos/chiroptology/10_IMG_3159.JPG" style="height:auto; width:99%">   
      </div>
  
      <div class="mySlides">
        <img src="/assets/photos/chiroptology/11_IMG_5163.JPG" style="height:auto; width:99%">  
      </div>
  
      <div class="mySlides">
        <img src="/assets/photos/chiroptology/12_IMG_0363.JPG" style="height:auto; width:99%">   
      </div>
  
      <div class="mySlides">
        <img src="/assets/photos/chiroptology/13_IMG_2666.JPG" style="height:auto; width:99%">   
      </div>
  
      <div class="mySlides">
        <img src="/assets/photos/chiroptology/14_IMG_1759.JPG" style="height:auto; width:99%">   
      </div>
  
      <div class="mySlides">
        <img src="/assets/photos/chiroptology/15_IMG_5222.JPG" style="height:auto; width:99%">   
      </div>
      
      <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
      <a class="next" onclick="plusSlides(1)">&#10095;</a>
  
      <div class="caption-container">
        <p id="caption"></p>
      </div>
    </div>
  </div>
</div>

<script>
  // Get the modal and slideshow elements
  var modal = document.getElementById('myModal');
  var closeButton = modal.querySelector('.close');

  // Slideshow variables
  var slideIndex = 1;

  // Function to open the modal and show the slideshow
  function openModal() {
    modal.style.display = 'block';
    showSlides(slideIndex);
  }

  // Function to close the modal
  function closeModal() {
    modal.style.display = 'none';
  }

  // Function to navigate to the next or previous slide
  function plusSlides(n) {
    showSlides(slideIndex += n);
  }

  // Function to show a specific slide
  function currentSlide(n) {
    showSlides(slideIndex = n);
  }

  // Function to display slides
  function showSlides(n) {
    var i;
    var slides = document.getElementsByClassName("mySlides");
    if (n > slides.length) { slideIndex = 1 }
    if (n < 1) { slideIndex = slides.length }
    for (i = 0; i < slides.length; i++) {
      slides[i].style.display = "none";
    }
    slides[slideIndex - 1].style.display = "block";
  }

  // Event listener for closing the modal
  closeButton.addEventListener('click', closeModal);

  // Close modal if clicked outside the slideshow content
  modal.addEventListener('click', function(event) {
    if (event.target === modal) {
      closeModal();
    }
  });

  // Close modal on pressing Escape key
  document.addEventListener('keydown', function(event) {
    if (event.key === 'Escape' && modal.style.display === 'block') {
      closeModal();
    }
    
    // Keyboard navigation for slideshow
    if (modal.style.display === 'block') {
      if (event.key === 'ArrowLeft') {
        plusSlides(-1);
      } else if (event.key === 'ArrowRight') {
        plusSlides(1);
      }
    }
  });
    
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
