<template>
  <div class="container">
      <div class="hero-content">
        <!--<p>Coming Soon</p>
        <img class="gps" src="../assets/gps.svg" alt=""> -->
      </div>
      <div class="text-row full color">
        <h3>The Vision</h3>
        <!-- <div class="line"></div> -->
        <p class="max">Indo Villas is a luxury residential enclave located in Avellanas with a collection of one and two-bedroom villas just steps from the Pacific Ocean. 
          The objective of Indo Villas is to create an intimate community that fulfills the lifestyle, travel, and wellness aspirations of the clientele spending more 
          time in this special region of Costa Rica. </p>
      </div>
      <div class="split-peak">
        <img src="../assets/split-peak-1.jpg" alt="">
      </div>
      <div class="split-mobile">
        <img src="../assets/split-peak-2.jpg" alt="">
      </div>
      <div class="text-row full white">
        <h3>Why Avellanas?</h3>
        <p class="max">Avellanas and its neighboring communities are buzzing with international, as well as local, ecotourism that is commanding luxury accommodations, 
          inspiring food & beverage venues, immediate access to world-class waves, and attractive amenities emphasizing wellness as well as sustainability. 
          The team at Indo Villas has recognized that there are insufficient options that match what the thriving ecotourism market is seeking in this 
          region and will fill that demand gap. Lastly, the timing is idyllic as the municipality has begun to pave the final section of roads which connects all of 
          the premier beach communities and grants streamlined accessibility as well as infrastructure enhancements.</p>
      </div>
      <VillaGallery />
      <div class="flex-box">
        <div class="left-box">
         <div class="left-text">
            <h5>AVELLANAS</h5>
            <h3>Exceptional Location.<br><span>Unrivaled Lifestyle.</span></h3>
          </div>
        </div>  
        <div class="right-image"></div>
      </div>
      <div class="flex-box reverse">
        <div class="left-image"></div>
        <div class="right-box">
         <div class="right-text">
            <h3>The Location<br><span></span></h3>
            <p>At Indo Villas, the location is the ethos of the new enclave. You, your guests, and your future renters are a 2-minute walk to some of Costa Rica's 
              most stunning white sand beaches as well as a world-class beach break with year-round waves. These homes will offer carefree access to half a dozen 
              of Costa Rica's best surf spots including Playa Negra, Little Hawaii, El Estero, Junquillal, and many more. In short, this stretch of coastline can be 
              considered Costa Rica's 7-Mile Miracle, and Indo Villas are positioned directly in the heart of it.</p>
          </div>
        </div>  
      </div>
      <LifestyleGallery />
      <div class="text-row full color contact" id="contact">
        <h3>Learn More About The Community</h3>
        <a href="mailto:trevor.capozza@gmail.com">GET IN TOUCH</a>
      </div>
   <!-- <div class="schematic max">
      <img src="../assets/schematics.png" alt="Schematics">
    </div> -->
  </div>
</template>

<script>
import LifestyleGallery from '../components/LifestyleGallery.vue'
import VillaGallery from '../components/VillaGallery.vue'

export default {
  name: 'HomeView',
  components: {
    LifestyleGallery,
    VillaGallery,
  }
}
</script>
