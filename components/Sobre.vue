<template>
  <div class="container-sobre">
    <div class="titulo">
      <h1>SOBRE</h1>
      <h2>A CASA DO VIDRO</h2>
    </div>
    <div class="conteudo-sobre">
      <div class="text-sobre">
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem
          maiores dolore, explicabo magnam voluptas delectus rem in, tempore
          neque accusamus reiciendis? Officia, laudantium quam. A, similique?
          Sunt saepe minus eligendi.
        </p>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem
          maiores dolore, explicabo magnam voluptas delectus rem in, tempore
          neque accusamus reiciendis? Officia, laudantium quam. A, similique?
          Sunt saepe minus eligendi.
        </p>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem
          maiores dolore, explicabo magnam voluptas delectus rem in, tempore
          neque accusamus reiciendis? Officia, laudantium quam. A, similique?
          Sunt saepe minus eligendi.
        </p>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem
          maiores dolore, explicabo magnam voluptas delectus rem in, tempore
          neque accusamus reiciendis? Officia, laudantium quam. A, similique?
          Sunt saepe minus eligendi.
        </p>
      </div>
      <div class="image-sobre">
        <img src="@/assets/images/loja.jpg" alt="" />
      </div>
    </div>
    <div class="btn-container">
      <button class="btn">Saiba Mais</button>
    </div>
    <div class="cards" >
      <div class="card" v-for="card in imgCard" :key="card">
        <img class="img-card" :src="card.img" alt="">
        <h3 class="text-card">{{ card.text }}</h3>
      </div>
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
};
</script>

<style scoped>
.titulo {
  text-align: center;
  font-weight: bold;
  margin: 60px 0;
}
.titulo h1 {
  font-size: 3.8rem;
  color: #309ac7;
}
.titulo h2 {
  margin-left: 180px;
  font-size: 1.6rem;
}

.conteudo-sobre {
  display: flex;
  justify-content: center;
}

.text-sobre {
  width: 500px;
  margin-right: 70px;
}
.text-sobre p {
  font-size: 1rem;
  text-align: justify;
  margin-bottom: 25px;
}
.image-sobre img {
  width: 700px;
  height: 400px;
}

</style>
