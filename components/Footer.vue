<template>
  <div class="container-footer">
    <div class="logo">
      <img src="@/assets/images/logo.png" alt="" />
      <p class="titulo">Siga nossos canais</p>
      <div class="redes-sociais">
        <i class="fa-brands fa-2x fa-instagram"></i>
        <i class="fa-brands fa-2x fa-facebook-f"></i>
      </div>
    </div>
    <div class="institucional">
      <ul>
        <p class="titulo">Institucional</p>
        <li><nuxt-link to="/">Home</nuxt-link></li>
        <li><nuxt-link to="/sobre">Sobre</nuxt-link></li>
        <li><nuxt-link to="/servicos">Serviços</nuxt-link></li>
        <li><nuxt-link to="/contatos">Contatos</nuxt-link></li>
        <li><nuxt-link to="/time">Nosso time</nuxt-link></li>
      </ul>
    </div>
    <div class="servicos">
      <ul>
        <p class="titulo">servicos</p>
        <li><nuxt-link to="/">Box em vidro</nuxt-link></li>
        <li><nuxt-link to="/">Sacadas</nuxt-link></li>
        <li><nuxt-link to="/">Espelhos</nuxt-link></li>
        <li><nuxt-link to="/">Cobertura em vidro</nuxt-link></li>
      </ul>
    </div>
    <div class="contato">
      <p class="titulo">Contato</p>
      <p class="contatos-infos">
        <fa class="icones" icon="phone-flip" /> <nuxt-link to="/">(44) 3253-9999</nuxt-link>
      </p>

      <p class="contatos-infos">
        <fa class="icones" :icon="['fab', 'whatsapp']" />
        <nuxt-link to="/">(44) 99999-9999</nuxt-link>
      </p>
      <p class="contatos-infos">
        <fa class="icones" icon="clock" /> <span>Seg - Sex: 8:00 - 18:00</span>
      </p>
    </div>
    <div class="contato">
      <h1>MAPA</h1>
      <h1>MAPA</h1>
      <h1>MAPA</h1>
    
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.container-footer {
  width: 100vw;
  height: 400px;
  background: #0b232e;
  display: flex;
  align-items: center;
  justify-content: center;
}
.redes-sociais {
  width: 140px;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: space-evenly;
}
.redes-sociais i {
  font-size: 33px;
  font-weight: 500;
  transition: all 0.2s ease-in-out;
  color: white;
  cursor: pointer;
}
.redes-sociais i:hover {
  transform: scale(1.2);
    color: #309ac7;
}
.titulo {
  color: #309ac7;
  font-size: 1.1rem;
  text-transform: uppercase;
  font-weight: bold;
  margin-bottom: 20px;
}

.logo img {
  margin-bottom: 20px;
  border-radius: 10px;
}
a {
  color: white;
  font-weight: bold;
  transition: all .3s;
}
a:hover{
  color: #309ac7;
}
.icones, .contatos-infos span{
  color: white;
}
.logo, .institucional, .servicos, .contato {
  width: 300px;
  height: 200px;
  display: flex;
  align-items: center;
  flex-direction: column;
  border-right: 1px solid rgba(255, 255, 255, 0.322);
}

ul li, .contatos-infos {
  margin-bottom: 10px;
}

</style>
