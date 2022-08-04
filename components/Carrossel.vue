<template>
  <div class="container-carrossel">
    <div class="arrows">
      <span @click="backCarrossel" class="arrow-left">&#8678;</span>
      <span class="arrow-rigth">&#8680;</span>
    </div>
    <div class="overlay"></div>
    <div class="carrossel">
      <transition :appear="true">
        <img :src="images[settings.imageIndex]" alt="">
      </transition>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      settings: {
        imageIndex: 0,
        autoplay: true,
        autoplaySpeed: 2000,
      },
      images: [
        require('@/assets/images/carrossel-1.jpg'),
        require('@/assets/images/carrossel-2.jpg'),
        require('@/assets/images/carrossel-3.jpg'),
        require('@/assets/images/carrossel-4.jpg'),
        require('@/assets/images/carrossel-5.jpg'),
        require('@/assets/images/carrossel-6.jpg')
      ]
    }
  },
  methods: {
    backCarrossel() {
      if(this.settings.imageIndex >= this.images.length -1) {
        this.settings.imageIndex = 0
      }else {
        this.settings.imageIndex++
      } 
    }
  }
}
</script>

<style>
.v-enter, .v-leave-to {

}
.v-enter-to, .v-leave{
  transform: translateX(-100%);
}
.v-enter-active, .v-leave-active {
  transition: all 3s;
}

.container-carrossel {
  display: flex;
  overflow: hidden ;
}
.carrossel {
  width: 100vw;
  height: 500px;
  transition: all 3s;
}
.arrows {
  width: 100vw;
  height: 500px;
  display: flex;
  justify-content: space-between;
  padding-left: 20px;
  padding-right: 20px;
  align-items: center;
  position: absolute;
}
.arrow-left, .arrow-rigth {
  font-size: 3rem;
  color: white;
  z-index: 2;
}
.overlay {
  width: 100vw;
  height: 500px;
  z-index: 1;
  position: absolute;
  background-color: rgba(0,0,0,.5)
}
.carrossel img {
  width: 100vw;
  height: 100%;
  background-position: center;
  object-fit: cover;
  transition: all 3s;
}

</style>