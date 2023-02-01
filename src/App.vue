<template>
    <div class="container">
      <div class="nav-bar">
        <img class="logo" alt="INDO logo" src="./assets/logo-horizontal-dark.svg">
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
