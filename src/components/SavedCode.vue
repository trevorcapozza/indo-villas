<template>
    <div>
        <div class="image-container">
            <img v-for="(image, index) in images" :src="image" :key="index"/>
        </div>
        <button @click="scrollImagesToEnd">Start</button>
        <button @click="scrollImagesToStart">End</button>
    </div>
</template>

<script>
  export default {
    data() {
      return {
        images: [
            require('../assets/image-gallery/adventure.jpg'),
            require('../assets/image-gallery/beach-day.jpg'),
            require('../assets/image-gallery/breakfast.jpg'),
            require('../assets/image-gallery/bw-barrell.jpg'),
            require('../assets/image-gallery/sunrise.jpg'),
            require('../assets/image-gallery/surf-check.jpg'),
            require('../assets/image-gallery/wellness-2.jpg'),
            require('../assets/image-gallery/wellness.jpg'),
        ],
      }
    },
    methods: {
        scrollImagesToEnd() {
            // Select the image container
            const imageContainer = document.querySelector('.image-container');

            // Scroll the images to the right by the width of the container
            imageContainer.scroll({
                left: imageContainer.scrollWidth,
                behavior: 'smooth'
            });
        },
        scrollImagesToStart() {
            // Select the image container
            const imageContainer = document.querySelector('.image-container');

            // Scroll the images to the left by the width of the container
            imageContainer.scroll({
                left: 0,
                behavior: 'smooth'
            });
        }
    }
  }
</script>    


<style>
.image-container {
  display: flex;
  align-items: center;
  overflow-x: hidden;
}

img {
  width: 25%;
  padding: 30px;
}

.caption {
  width: 25%;
  text-align: center;
}
</style>