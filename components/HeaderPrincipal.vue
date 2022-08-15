<template>
  <div class="container-header-principal">
    <div class="logo">
      <nuxt-link to="/"><img src="../assets/images/logo.png" alt="" /></nuxt-link>
    </div>
    <div class="redes-sociais">
      <i class="fa-brands fa-2x fa-instagram"></i>
      <i class="fa-brands fa-2x fa-facebook-f"></i>
    </div>
    <nav>
      <ul>
        <li><nuxt-link class="menu-itens" to="/">Inicio</nuxt-link></li>
        <li><nuxt-link class="menu-itens" href="#sobre" to="#sobre">Sobre</nuxt-link></li>
        <li><nuxt-link class="menu-itens" to="#servicos">Serviços</nuxt-link></li>
        <li><nuxt-link class="menu-itens" to="/contato">Contato</nuxt-link></li>
        <li><nuxt-link class="menu-itens" to="/time">Nosso Time</nuxt-link></li>
      </ul>
    </nav>
  </div>
</template>

<script>

export default {
};
</script>

<style scoped>
.container-header-principal {
  width: 100vw;
  max-width: 1200px;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  height: 90px;
  margin: 0 auto;
}
.logo {
  width: 70px;
  height: 70px;
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
  transition: all 0.5s;
}
.redes-sociais i:hover {
  background: #309ac7;
  color: white;
}
nav {
  width: 500px;
}
ul {
  display: flex;
  justify-content: space-around;
  align-items: center;
}

.menu-itens {
  color: #0b0e11;
  font-family: "Montserrat";
  font-size: 1.1rem;
  letter-spacing: 1px;
  background-image: linear-gradient(to right, #54b3d6, #54b3d6 50%, #000 50%);
  background-size: 200% 100%;
  background-position: -100%;
  display: inline-block;
  padding: 5px 0;
  position: relative;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  transition: all 0.3s ease-in-out;
}

.menu-itens:before {
  content: "";
  background: #54b3d6;
  display: block;
  position: absolute;
  bottom: -3px;
  left: 0;
  width: 0;
  height: 3px;
  transition: all 0.3s ease-in-out;
}
.menu-itens:hover {
  background-position: 0;
}

.menu-itens:hover::before {
  width: 100%;
}
</style>
