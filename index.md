---
layout: single
author_profile: true
permalink: /
sidebar:
  nav: ""  
---

I’m a highly motivated Ph.D. candidate in Computational Mathematics with a strong background in scientific computing, numerical modeling, data assimilation and inverse methods. My research focuses on modeling complex physical systems, particularly wildfire smoke transport, by combining high-performance computing with techniques from data assimilation and inverse problems. I enjoy building and testing algorithms, running large-scale simulations, and working across disciplines to solve real-world problems. Sharing my work through writing and presentations has also been a key part of my growth as a researcher.

<div class="research-slideshow">
  <div class="slideshow-container">
    <div class="slide active">
      <img src="/assets/images/image_5.jpg" alt="Wildfire Smoke Modeling">
<!-- <div class="slide-caption">
        <h3>Wildfire Smoke Modeling</h3>
        <p>Advanced computational techniques for smoke transport prediction</p>
      </div> -->
    </div>
    
    <div class="slide">
      <img src="/assets/images/image_1.jpg" alt="Data Assimilation">
     <!-- <div class="slide-caption">
        <h3>Wildfire Smoke Modeling</h3>
        <p>Advanced computational techniques for smoke transport prediction</p>
      </div> -->
    </div>
    
    <div class="slide">
      <img src="/assets/images/image_2.jpg" alt="Computational Mathematics">
      <!-- <div class="slide-caption">
        <h3>Wildfire Smoke Modeling</h3>
        <p>Advanced computational techniques for smoke transport prediction</p>
      </div> -->
    </div>

    <div class="slide">
      <img src="/assets/images/image_3.jpg" alt="Computational Mathematics">
      <!-- <div class="slide-caption">
        <h3>Wildfire Smoke Modeling</h3>
        <p>Advanced computational techniques for smoke transport prediction</p>
      </div> -->
    </div>
    
    <!-- Navigation arrows -->
    <button class="prev" onclick="changeSlide(-1)">&#10094;</button>
    <button class="next" onclick="changeSlide(1)">&#10095;</button>
  </div>
  
  <!-- Dots indicator -->
  <div class="dots-container">
    <span class="dot active" onclick="currentSlide(1)"></span>
    <span class="dot" onclick="currentSlide(2)"></span>
    <span class="dot" onclick="currentSlide(3)"></span>
    <span class="dot" onclick="currentSlide(4)"></span>
  </div>
</div>

<style>
.research-slideshow {
  max-width: 700px; /* Increased width */
  margin: 20px auto;
  position: relative;
}

.slideshow-container {
  position: relative;
  background: #f8f9fa;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}

.slide {
  display: none;
  position: relative;
}

.slide.active {
  display: block;
}

.slide img {
  width: 100%;
  height: auto; /* Let height adjust naturally */
  max-height: 500px; /* Set maximum height */
  object-fit: contain;
  background-color: #f8f9fa;
  display: block;
}

.slide-caption {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background: linear-gradient(transparent, rgba(0,0,0,0.8));
  color: white;
  padding: 30px 20px 15px;
}

.slide-caption h3 {
  margin: 0 0 5px 0;
  font-size: 1.2em;
}

.slide-caption p {
  margin: 0;
  font-size: 0.9em;
  opacity: 0.9;
}

/* Navigation arrows */
.prev, .next {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  background: rgba(0,0,0,0.5);
  color: white;
  border: none;
  padding: 15px 18px;
  font-size: 18px;
  cursor: pointer;
  border-radius: 0 3px 3px 0;
  transition: background-color 0.3s;
  z-index: 10;
}

.next {
  right: 0;
  border-radius: 3px 0 0 3px;
}

.prev:hover, .next:hover {
  background: rgba(0,0,0,0.8);
}

/* Dots indicator */
.dots-container {
  text-align: center;
  padding: 15px 0;
}

.dot {
  height: 12px;
  width: 12px;
  margin: 0 5px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  cursor: pointer;
  transition: background-color 0.3s;
}

.dot.active, .dot:hover {
  background-color: #717171;
}

/* Responsive design */
@media (max-width: 768px) {
  .research-slideshow {
    max-width: 95%;
  }
  
  .slide img {
    max-height: 400px;
  }
  
  .prev, .next {
    padding: 12px 15px;
    font-size: 16px;
  }
}
</style>

<script>
let slideIndex = 0;

function changeSlide(n) {
  showSlide(slideIndex += n);
}

function currentSlide(n) {
  showSlide(slideIndex = n - 1);
}

function showSlide(n) {
  const slides = document.querySelectorAll('.slide');
  const dots = document.querySelectorAll('.dot');
  
  if (n >= slides.length) { slideIndex = 0; }
  if (n < 0) { slideIndex = slides.length - 1; }
  
  // Hide all slides
  slides.forEach(slide => slide.classList.remove('active'));
  dots.forEach(dot => dot.classList.remove('active'));
  
  // Show current slide
  slides[slideIndex].classList.add('active');
  dots[slideIndex].classList.add('active');
}

// Optional: Auto-advance slides every 5 seconds
setInterval(() => {
  changeSlide(1);
}, 5000);
</script>

**Recent Research**  
Improving wildfire smoke forecast accuracy through data assimilation and model error quantification.


## Latest Updates 
Explore: [How Accurate Are Smoke Forecasts?](/2025/07/07/how-accurate-are-smoke-forecasts/)


**I'M STILL DEVELOPING THIS SITE!**
