<template>
  <transition name="slide-in">
    <div
      class="carrossel-itens"
      v-show="imageIndex === index"
    >
      <img :src="slide" />
    </div>
  </transition>
</template>

<script>
export default {
  props: ["slide", "imageIndex", "index"],
};
</script>

<style scoped>
.carrossel-itens {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
}
.carrossel-itens img {
  width: 100vw;
  height: 100%;
  object-fit: cover;
}

.slide-in-enter-active,
.slide-in-leave-active {
  transition: all 2s ease-in-out;
}
.slide-in-enter {
  opacity: 0;
  transform: scale(1.5);

}
.slide-in-leave-from {
  opacity: 1;
  transform: scale(1.5);
}
</style>