<template>
    <div class="container">
      <div class="nav-bar">
        <img class="logo" alt="INDO logo" src="./assets/logo-horizontal.svg">
        <div class="links">
          <a href="#villas">The Villas</a>
          <a href="#contact">Contact</a>
        </div>
      </div>  
    </div>
  <!--- <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </nav> --->
  <router-view/>
  <FooterView />
</template>


<script>
import FooterView from './components/FooterView.vue'

export default {
   components: {
    FooterView
   }, 
  }
</script>

<style src="@/css/main.scss" lang="scss" />
