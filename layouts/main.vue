<template>
  <div class="container">
    <div class="header">
      <HeaderContatos />
      <HeaderPrincipal />
    </div>
    <div class="conteudo">
      <Nuxt />
    </div>
    <Footer />
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.conteudo {
  padding-top: 140px;
}
.header {
  position: fixed;
  z-index: 999;
  background: rgb(255, 255, 255);
  border-bottom: 1px solid black;

}
</style>
