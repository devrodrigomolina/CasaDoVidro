<template>
  <transition name="carrossel" >
    <div class="carrossel" v-show="index == imageIndex  ">
      <img :src="slide" alt="" />
    </div>
  </transition>
</template>

<script>
export default {
  props: {
    slide: Array, String,
    index: Number,
    imageIndex: Number,
  },
}
</script>

<style scoped>
.carrossel-enter-active,
.carrossel-leave-active {
  transition: all 3s ease-in-out;
}
.carrossel-enter-from {
  transform: translateX(-100%);
}
.carrossel-leave-to {
  transform: translateX(100%);
  z-index: 2;
}

.carrossel {
  width: 100vw;
  height: 500px;
  position: absolute;
}
.carrossel img {
  width: 100vw;
  height: 100%;
  object-fit: cover;
}
</style>