<template>
  <div class="container-header-principal">
    <div class="logo">
      <img src="../assets/images/logo.jpg" alt="">
    </div>
    <div class="redes-sociais">
      <i class="fa-brands fa-2x fa-instagram"></i>
      <i class="fa-brands fa-2x fa-facebook-f"></i>
    </div>
    <nav>
      <ul>
        <li>Inicio</li>
        <li>Sobre</li>
        <li>Serviços</li>
        <li>Contato</li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.container-header-principal {
  width: 100vw;
  max-width: 1400px;
  display: flex;
  justify-content: space-around;
  align-items: center;
  height: 80px;
  margin: 0 auto;
  border: 1px solid red;
}
.logo {
  width: 80px;
  height: 80px;
}
.logo img {
  height: 100%;
}
.redes-sociais {
  display: flex;
}
nav {
  width: 500px;
}
ul {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
</style>