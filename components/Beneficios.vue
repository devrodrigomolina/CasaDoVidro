<template>
  <div class="container-beneficios">
    <div class="titulo">
      <h1>BENEFICIOS DA ARQUITETURA EM VIDRO</h1>
    </div>
    <div class="cards">
      <div class="card" v-for="card in infosCards" :key="card">
        <img class="img-card" :src="card.img" alt="">
        <p class="text-card">{{ card.text }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      infosCards: [
        {
          img: require("@/assets/images/sun.png"),
          text: 'Evita Luminosidade Excessiva'
        },
        {
          img: require("@/assets/images/mute.png"),
          text: 'Proporciona Isolamento Acústico'
        },
        {
          img: require("@/assets/images/diamond.png"),
          text: 'Economize Energia com Iluminação Natural'
        },
        {
          img: require("@/assets/images/power.png"),
          text: 'Valoriza a estética de seu ambiente'
        },
        {
          img: require("@/assets/images/value.png"),
          text: 'Proporciona um visual mais moderno'
        },
      ],
    }
  }
}
</script>

<style scoped>
.container-beneficios {
  width: 100vw;
}
.titulo {
  text-align: center;
}
.cards {
  display: flex;
  align-items: center;
}
.card {
  width: 240px;
}
.card img {
  width: 80px;
  height: 80px;
  margin: 30px 0;
}
.card p {
  text-align: center;
  font-size: 1.1rem;
  margin: 20px 20px;
}
</style>