<template>
    <div class="lifestyle color">
        <div class="title">
            <h3>The Villas</h3>
            <div class="buttons">
                <i class="fa-regular fa-chevron-left left" @click="scrollImagesToStart"></i>
                <i class="fa-regular fa-chevron-right right" @click="scrollImagesToEnd"></i>
            </div>
        </div>
        <div class="container-7">
            <div class="image-container">
                <img src="../assets/villa-gallery/bathroom.jpg" alt="caption1" />
                <!-- <h6>Secluded Volcanic Beaches</h6>
                <p>Avellanas is home to some of the most beautiful beaches.</p> -->
            </div>
            <div class="image-container">
                <img src="../assets/villa-gallery/bedroom.jpg" alt="caption2" />
                <!-- <h6>Tradewinds at Local Reefs</h6>
                <p>Take a day trip from your villa and surf one of the world's most famous waves.</p> -->
            </div>
            <div class="image-container">
                <img src="../assets/villa-gallery/kitchen.jpg" alt="caption3" />
                <!-- <h6>Breakfast at the Beach</h6>
                <p>Wake up and enjoy a lovely breakfast just down the road at Cafe Corazon.</p> -->
            </div>
            <div class="image-container">
                <img src="../assets/villa-gallery/livingroom.jpg" alt="caption4" />
                <!-- <h6>Layday Exploration</h6>
                <p>Spend a day hiking through the mountains to some of the most peaceful waterfalls.</p> -->
            </div>
            <div class="image-container">
                <img src="../assets/villa-gallery/stairs.jpg" alt="caption5" />
                <!-- <h6>Rejuvenation</h6>
                <p>Spend a day relaxing on the beach with your friends.</p> -->
            </div>
      </div>
    </div>
  </template>

<script>

export default {
    data() {

    },
    methods: {
        scrollImagesToEnd() {
          // Select the image container
          const imageContainer = document.querySelector('.container-7');
                
          // Get the width of the viewport
          const viewportWidth = window.innerWidth;
                
          // Scroll the images to the right by the width of the viewport
          imageContainer.scrollBy({
            left: viewportWidth,
            behavior: 'smooth'
          });
        },
        scrollImagesToStart() {
          // Select the image container
          const imageContainer = document.querySelector('.container-7');
        
          // Get the width of the viewport
          const viewportWidth = window.innerWidth;
        
          // Scroll the images to the left by the width of the viewport
          imageContainer.scrollBy({
            left: -viewportWidth,
            behavior: 'smooth'
          });
        }     
}



}

</script>
  