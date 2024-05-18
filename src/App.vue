<template>

<q-layout>
  <Navbar />
  <q-page-container>
   
    <q-page>
      <Carousel />
      <Card />
    </q-page>
    <Footer />
  </q-page-container>

</q-layout>

</template>
<script setup>
import Navbar from './components/Navbar.vue';
import Footer from './components/Footer.vue';
import Carousel from './components/Carousel.vue';
import Card from './components/Card.vue';
</script>