<template>
  <div class="q-pa-md">
    <q-carousel
      animated
      v-model="slide"
      navigation
      infinite
      :autoplay="autoplay"
      arrows 
      transition-prev="slide-right"
      transition-next="slide-left"
      @mouseenter="autoplay = false"
      @mouseleave="autoplay = true"
    >
      <q-carousel-slide :name="1" class="carousel-slide" img-src="https://img.id.my-best.com/product_images/e7e81428df597f577ed05144cd91c4ed.png?ixlib=rails-4.3.1&q=70&lossless=0&w=800&h=800&fit=clip&s=30afa350ee1530e3c1dbaac1d445771b" />
      <q-carousel-slide :name="2" class="carousel-slide" img-src="https://ae01.alicdn.com/kf/S9a762acc52d047b6a83f11d6ff240fc43/Headset-Telinga-Kucing-Biru-Merah-Muda-Headphone-Anak-Perempuan-Kitty-untuk-Anak-Headset-Bluetooth-Nirkabel-dengan.jpg" />
      <q-carousel-slide :name="3" class="carousel-slide" img-src="https://planetcomputer.co.id/cdn/shop/products/73e9d303-e080-4a6c-be27-62b19b5d48c6_56f059f9-e3d0-4947-bfe9-9080971af5f3_800x.jpg?v=1658825188" />
      <q-carousel-slide :name="4" class="carousel-slide" img-src="https://www.static-src.com/wcsstore/Indraprastha/images/catalog/full//100/MTA-45182709/tidak_ada_merk_baju_kaos_dsitro_pria_smile_full01_kc7rygnm.jpg" />
    </q-carousel>
  </div>
</template>

<script>
import { ref } from 'vue'

export default {
  setup() {
    return {
      slide: ref(1),
      autoplay: ref(true)
    }
  }
}
</script>

<style scoped>
.carousel-slide img {
  width: 100%; /* Contoh pengaturan lebar */
  height: auto; /* Menjaga aspek rasio */
  max-height: 400px; /* Contoh batasan tinggi maksimal */
  object-fit: cover; /* Menjaga gambar agar tidak terdistorsi */
}
</style>
