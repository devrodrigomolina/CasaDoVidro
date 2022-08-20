<template>
  <div id="sobre" class="container-sobre">
    <div class="titulo">
      <h1>SOBRE</h1>
      <h2>A CASA DO VIDRO</h2>
    </div>
    <div class="conteudo-sobre">
      <div class="text-sobre">
        <p>
          Fundada em 1996, é pioneira em soluções de vidros e espelhos para marcenarias na região de Maringá, interior do Paraná, tornando-se desde cedo, uma empresa de qualidade ímpar e totalmente inovadora, capaz de suprir todas as necessidades de seus clientes em diversas áreas que atuam com envidraçamento, seja para fim arquitetônico ou decorativo.
        </p>
        <p>
         Empresa consolidada no ramo, realizando o sonho de seus clientes há mais de 26 anos e operando apenas com maquinário de última geração, resultando em um serviço de acabamento impecável. Tudo isso sem deixar de lado a preocupação com o meio-ambiente, contando com um sistema de abastecimento pluvial que colabora de forma positiva á economia da água necessária ao processo industrial.
        </p>
        <p>
          Atendimento especializado para lojas de decoração, painéis espelhados, vidros pintados, comumente utilizados no acabamento de móveis decorativos. Venha conhecer a Casa do vidro!
        </p>

      </div>
      <div class="image-sobre">
        <img src="@/assets/images/loja.jpg" alt="" />
      </div>
    </div>
    <Button />
    <CardsSobre />
  </div>
</template>

<script>
export default {

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
  position: relative;
}
.titulo h2::before {
  content: '';
  width: 140px;
  height: 3px;
  background: #309ac7;
  position: absolute;
  bottom: -20px;
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
.image-sobre {
  width: 700px;
}
.image-sobre img {
  width: 100%;
}

</style>
