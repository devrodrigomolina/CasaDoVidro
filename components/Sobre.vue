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
}
</style>
