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
    <div class="cards">
      <div class="card-1">
        <img class="img-card" src="@/assets/images/shield.png" alt="">
        <h3 class="text-card">3 Anos de garantia de serviço</h3>
      </div>
      <div class="card-2">
        <img class="img-card" src="@/assets/images/shield-1.png" alt="">
        <h3 class="text-card">5 Anos de garantia da fabrica</h3>
      </div>
      <div class="card-3">
        <img class="img-card" src="@/assets/images/credit-card.png" alt="">
        <h3 class="text-card">Pagamento em até 12x sem juros</h3>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
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
.btn-container {
  display: flex;
  justify-content: center;
  margin: 60px 0;
}
.btn {
  width: 250px;
  height: 50px;
  border-radius: 50px;
  background: #309ac7;
  color: white;
  font-size: 1rem;
  border: none;
  text-align: center;
  font-weight: bold;
  transition: all .3s;
  cursor: pointer;
}
.btn:hover {
  background: #186383;
  transform: translateY(-10px);
}

.cards {
  width: 100vw;
  max-width: 1300px;
  margin: 130px auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.img-card {
  width: 80px;
  height: 80px;
  margin: 25px 0;
}
.card-1,.card-2,.card-3 {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  width: 350px;
  height: 230px;
  background: #186383;
  border-radius: 10px;
  border: 1px solid rgba(0, 0, 0, 0);
  box-shadow:0px 0px 0px 5px rgb(255, 255, 255) inset;
  transition: all .3s;
} 
.text-card {
  color: rgba(255, 255, 255, 0.884);
}
.card-1:hover,.card-2:hover,.card-3:hover {
  transform: translateY(-10px);
} 
</style>
