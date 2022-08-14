<template>
  <div class="btn-container">
    <button class="btn">Saiba Mais</button>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
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
</style>