<template>
  <div class="q-pa-md">
    <div class="grid-wrapper q-gutter-md">
      <q-card v-for="(card, index) in cards" :key="index" class="my-card">
        <img :src="card.img" class="card-img">
        <q-card-section>
          <div class="text-h6">{{ card.title }}</div>
          <div class="text-subtitle2">{{ card.subtitle }}</div>
        </q-card-section>
        <q-card-section class="q-pt-none">
          {{ card.description }}
        </q-card-section>
      </q-card>
    </div>
  </div>
</template>

<script>
export default {
  setup() {
    return {
      cards: [
        {
          img: "https://cdn.consina.com/wp-content/uploads/2021/08/boulder-GY-800x800-1.jpg",
          title: "Celana Training",
          subtitle: "Design By anonymous ",
          description: "Hanya celana Training biasa"
        },
        {
          img: "https://www.static-src.com/wcsstore/Indraprastha/images/catalog/full//100/MTA-45182709/tidak_ada_merk_baju_kaos_dsitro_pria_smile_full01_kc7rygnm.jpg",
          title: "Baju Grey",
          subtitle: "Design By anonymous ",
          description: "Baju yang desain keren"
        },
        {
          img: "https://planetcomputer.co.id/cdn/shop/products/73e9d303-e080-4a6c-be27-62b19b5d48c6_56f059f9-e3d0-4947-bfe9-9080971af5f3_800x.jpg?v=1658825188",
          title: "Mouse",
          subtitle: "Design By anonymous ",
          description: "Mouse tahan banting"
        },
        {
          img: "https://ae01.alicdn.com/kf/S9a762acc52d047b6a83f11d6ff240fc43/Headset-Telinga-Kucing-Biru-Merah-Muda-Headphone-Anak-Perempuan-Kitty-untuk-Anak-Headset-Bluetooth-Nirkabel-dengan.jpg",
          title: "Headphone",
          subtitle: "Design By anonymous ",
          description: "Headphone harga murah dengan kualitas super"
        },
        {
          img: "https://img.id.my-best.com/product_images/e7e81428df597f577ed05144cd91c4ed.png?ixlib=rails-4.3.1&q=70&lossless=0&w=800&h=800&fit=clip&s=30afa350ee1530e3c1dbaac1d445771b",
          title: "Keyboard",
          subtitle: "Design By anonymous ",
          description: "Keyboard yang bisa rgb"
        }
      ]
    };
  }
};
</script>

<style scoped>
.grid-wrapper {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  gap: 16px;
}
.my-card {
  width: 100%;
  max-width: 100%;
}
.card-img {
  width: 100%;
  height: auto;
}
</style>
