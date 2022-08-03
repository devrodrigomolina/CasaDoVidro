<template>
  <div class="container-header">
    <div class="header-contatos">
      <div class="infos-contatos">
  
        <p class="contatos-infos" >
          <fa class="icones" icon="phone-flip" /> <a href="">(44) 3253-9999</a>
        </p>
       
        <p class="contatos-infos">
          <fa class="icones" :icon="['fab', 'whatsapp']" /> <a href="">(44) 99999-9999</a>
        </p>
        <p class="contatos-infos">
          <fa class="icones" icon="clock" /> Seg - Sex: 8:00 - 18:00
        </p>
      </div>

      <div class="container-btn">
        <button class="btn">Solicite um orçamento</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
};
</script>

<style scoped>
.container-header {
  width: 100vw;
  height: 50px;
  background: rgb(26, 30, 36);
}
.icones {
  color: #309ac7;
}
.header-contatos {
  width: 1200px;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin: 0 auto;
}
.infos-contatos {
  width: 700px;
  display: flex;
  justify-content: space-around;
}
.contatos-infos, .contatos-infos a{
  font-weight: 600;
  color: white;
}
.container-btn {
  height: 100%;
}
.btn {
  width: 400px;
  height: 100%;
  background: #309ac7;
  font-weight: 800;
  border: none;
  cursor: pointer;
  border-radius: 4px;
  color: white;
  text-transform: uppercase;
  transition: all .5s;
}
.btn:hover {
  background: #186383;
}
</style>
