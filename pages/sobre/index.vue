<template>
 <div class="carrossel">

  <VueSlickCarousel v-bind="settings">
  <div v-for="img in images" :key="img">
    <img :src="img" />
  </div>
  </VueSlickCarousel>
 </div>
</template>

<script>
export  default {
 layout: 'main',
 data() {
  return {
    settings: {
        slidesToShow: 1,
        arrows: true,
        autoplay: true,
        autoplaySpeed: 1000,
        simple: true
      },
    images: [
        require("@/assets/images/carrossel-1.jpg"),
        require("@/assets/images/carrossel-2.jpg"),
        require("@/assets/images/carrossel-3.jpg"),
        require("@/assets/images/carrossel-4.jpg"),
        require("@/assets/images/carrossel-5.jpg"),
        require("@/assets/images/carrossel-6.jpg"),
      ],
  }
 }
}
</script>

<style scoped>
.carrossel {
  width: 100vw;
  max-width: 50vw;
  margin: 0 auto;
}
.carousel-wrapper {
  width: 800px;
  border: 1px solid red;
  height: 600px;
  padding: 40px;
  overflow: hidden;
}
img {
  margin: auto;
  width: 800px;
  background-image: linear-gradient(gray 100%, transparent 0);
}


</style>