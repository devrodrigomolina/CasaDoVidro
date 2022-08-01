<template>
  <div class="container-header">
    <div class="header-contatos">
      <div class="infos-contatos">
        <p class="contatos-infos">(44) 99999-9999</p>
        <p class="contatos-infos">(44) 3253-9999</p>
        <p class="contatos-infos">Seg - Sex: 8:00 - 18:00</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.header-contatos {
  width: 100vw;
  height: 60px;
  background: rgb(26, 30, 36);
}
.infos-contatos {
  width: 600px;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 0 auto;
  border: 1px solid red;
}
.contatos-infos {
  margin-left: 40px;
  font-weight: 600;
  color: white;
}
</style>