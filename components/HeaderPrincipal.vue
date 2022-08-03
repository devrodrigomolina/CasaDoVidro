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
        <li><a href="">Inicio</a></li>
        <li><a href="">Sobre</a></li>
        <li><a href="">Serviços</a></li>
        <li><a href="">Contato</a></li>
        <li><a href="">Contato</a></li>
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
  max-width: 1200px;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  height: 80px;
  margin: 0 auto;
}
.logo {
  width: 80px;
  height: 80px;
}
.logo img {
  height: 100%;
}
.redes-sociais {
  width: 140px;
  height: 100%;
  display: flex;
  align-items: center;
}
.redes-sociais i {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 80px;
  height: 60px;
  border-radius: 8px;
  font-size: 22px;
  font-weight: 500;
  transition: all .5s;
}
.redes-sociais i:hover {
  background: #309ac7;
  color: white;
}
nav {
  width: 500px;
  font-weight: 500;
}
ul {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
a {
  color: #0b0e11;
  font-family: 'Montserrat';
  font-size: 1.1rem;
}
a:hover {
  color: #309ac7;
}
</style>