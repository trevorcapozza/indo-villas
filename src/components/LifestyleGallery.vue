<template>
    <div class="lifestyle white">
        <div class="title">
            <h3>Lifestyle</h3>
            <div class="buttons">
                <i class="fa-regular fa-chevron-left left" @click="scrollImagesToStart"></i>
                <i class="fa-regular fa-chevron-right right" @click="scrollImagesToEnd"></i>
            </div>
        </div>
        <div class="container-8">
          <div class="image-container">
                <img src="../assets/image-gallery/the-view.jpg" alt="caption1" />
                <h6>The View</h6>
            </div>
            <div class="image-container">
                <img src="../assets/image-gallery/lifestyle-7.jpg" alt="caption1" />
                <h6>Secluded Volcanic Beaches</h6>
                <!-- <p>Avellanas is home to some of the most beautiful beaches.</p> -->
            </div>
            <div class="image-container">
                <img src="../assets/image-gallery/barrell-2.jpg" alt="caption2" />
                <h6>Tradewinds at Local Reefs</h6>
                <!-- <p>Take a day trip from your villa and surf one of the world's most famous waves.</p> -->
            </div>
            <div class="image-container">
                <img src="../assets/image-gallery/avocado-toast.jpg" alt="caption3" />
                <h6>Breakfast at the Beach</h6>
               <!-- <p>Wake up and enjoy a lovely breakfast just down the road at Cafe Corazon.</p> -->
            </div>
            <div class="image-container">
                <img src="../assets/image-gallery/lifestyle-3.jpg" alt="caption4" />
                <h6>Layday Exploration</h6>
               <!-- <p>Spend a day hiking through the mountains to some of the most peaceful waterfalls.</p> -->
            </div>
            <!--<div class="image-container">
                <img src="../assets/image-gallery/hanna.jpg" alt="caption5" />
                <h6>Rejuvenation</h6>
                <p>Spend a day relaxing on the beach with your friends.</p>
            </div> -->
            <!--<div class="image-container">
                <img src="../assets/image-gallery/lifestyle-4.jpg" alt="caption5" />
                <h6>Find Your Peak</h6>
                <p>Spend a day relaxing on the beach with your friends.</p>
            </div> -->
            <div class="image-container">
                <img src="../assets/image-gallery/coffee-3.jpg" alt="caption6" />
                <h6>Morning Ritual</h6>
               <!-- <p>Take an adventure through the rain forest and cool down in a natural pool.</p> -->
            </div>
            <div class="image-container">
                <img src="../assets/image-gallery/explore.jpg" alt="caption1" />
                <h6>The Search</h6>
                <!-- <p>Avellanas is home to some of the most beautiful beaches.</p> -->
            </div>
            <!-- <div class="image-container">
                <img src="../assets/image-gallery/lifestyle-5.jpg" alt="caption6" />
                <h6>Sand Bars Out Front</h6>
                <p>Walk right out your doorstep to a handful of perfect waves.</p>
            </div> -->
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
          const imageContainer = document.querySelector('.container-8');
                
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
          const imageContainer = document.querySelector('.container-8');
        
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
  