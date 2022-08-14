<template>
  <div class="cards" >
    <div class="card" v-for="card in imgCard" :key="card">
      <img class="img-card" :src="card.img" alt="">
      <h3 class="text-card">{{ card.text }}</h3>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      imgCard: [
        {
          img: require('@/assets/images/shield.png'),
          text: '3 Anos de garantia de serviço'
        },
        {
          img: require('@/assets/images/shield-1.png'),
          text: '5 Anos de garantia da fabrica'
        },
        {
          img: require('@/assets/images/credit-card.png'),
          text: 'Pagamento em até 12x sem juros'
        },
      ]
    }
  }
}
</script>

<style scoped>


</style>