<template>
  <div class="container-carrossel">
    <div class="carrossel-inner">
      <div class="overlay">
        <div class="infos">
          <h1>Modernidade</h1>
          <span>E Sofisticação</span>
        </div>
      </div>
      <CarrosselItens
        v-for="(img, index) in images"
        :key="`item-${index}`"
        :slide="img"
        :imageIndex="settings.imageIndex"
        :index="index"
      />
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
        autoplaySpeed: null,
      },
      images: [
        require("@/assets/images/carrossel-1.jpg"),
        require("@/assets/images/carrossel-2.jpg"),
        require("@/assets/images/carrossel-3.jpg"),
        require("@/assets/images/carrossel-4.jpg"),
        require("@/assets/images/carrossel-5.jpg"),
        require("@/assets/images/carrossel-6.jpg"),
      ],
    };
  },
  methods: {
    setImageIndex(index) {
      this.settings.imageIndex = index;
    },
  },

  mounted() {
    this.settings.autoplaySpeed = setInterval(() => {
      const index =
        this.settings.imageIndex < this.images.length - 1
          ? this.settings.imageIndex + 1
          : 0;
      this.setImageIndex(index);
    }, 6000);
  },
  beforeUnmount() {
    clearInterval(this.settings.autoplaySpeed);
  },
};
</script>

<style scoped>
.container-carrossel {
  display: flex;
  justify-content: center;
}
.carrossel-inner {
  position: relative;
  width: 100vw;
  height: 500px;
  overflow: hidden;
}

.overlay {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100vw;
  height: 500px;
  z-index: 4;
  position: absolute;
  background-color: rgba(0, 0, 0, 0.5);
}

.infos {
  text-align: center;
}
.infos h1 {
  color: white;
  font-size: 5rem;
}

.infos span { 
  font-weight: bold;
  font-size: 3rem;
  color: #309ac7;
}
</style>
