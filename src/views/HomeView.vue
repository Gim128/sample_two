<template>
  <div class="home">
    <div class="container">
      <NavbarComponent />
      <HeroSection /> 
      <CardSection/>
      <SliderSection />
    </div>
  </div>
 
</template>

<script setup>
import CardSection from '../components/CardSection.vue';
import HeroSection from '../components/HeroSection.vue';
import NavbarComponent from '../components/NavbarComponent.vue';
import SliderSection from '../components/SliderSection.vue';

  
</script>

<style scoped>

</style>