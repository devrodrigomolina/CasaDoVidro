<template>
  <div class="container-servicos">
    <div class="titulo-servicos">
      <h1>NOSSOS</h1>
      <h2>SERVIÇOS</h2>
    </div>
    <div class="servicos-itens">
      <div class="item">
        <div class="infos-img">
          <div class="info">
            <h2>Box de vidro</h2>
            <p>
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Fugiat
              omnis explicabo et dolor itaque hic placeat quis quo in esse
              provident pariatur, totam, nulla ratione consectetur eos
              reprehenderit. Cum, in! Lorem ipsum dolor sit amet consectetur
              adipisicing elit. Et laudantium ratione odit ad laboriosam error
              quidem, animi, illo quia adipisci, reprehenderit quibusdam.
              Impedit voluptatibus repellendus tempore beatae rerum quod
              consequatur! Lorem ipsum dolor sit amet consectetur adipisicing
              elit. Vel, animi, dignissimos numquam voluptatibus dolorem et
              velit temporibus harum esse blanditiis magni neque assumenda omnis
              ex placeat. Ab temporibus ducimus necessitatibus!
            </p>
            <Button />
          </div>
          <img src="@/assets/images/box.jpg" alt="" />
        </div>
      </div>
      <div class="item">
        <div class="infos-img">
          <img src="@/assets/images/corrimao.jpg" alt="" />
          <div class="info">
            <h2>Corrimão de vidro</h2>
            <p>
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Fugiat
              omnis explicabo et dolor itaque hic placeat quis quo in esse
              provident pariatur, totam, nulla ratione consectetur eos
              reprehenderit. Cum, in! Lorem ipsum dolor sit amet consectetur
              adipisicing elit. Non quia accusantium, pariatur sunt, voluptas
              odit, dolorem dolor iusto a inventore tempora illo facilis quis
              iste! Quae deserunt id minima beatae! Lorem ipsum dolor sit amet
              consectetur adipisicing elit. Quas neque veritatis, at nemo odio
              recusandae quidem illum voluptate officiis pariatur, omnis minima
              praesentium vitae iure. Eaque voluptates labore sint amet.
            </p>
            <Button />
          </div>
        </div>
      </div>
      <div class="item">
        <div class="infos-img">
          <div class="info">
            <h2>Espelho</h2>
            <p>
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Fugiat
              omnis explicabo et dolor itaque hic placeat quis quo in esse
              provident pariatur, totam, nulla ratione consectetur eos
              reprehenderit. Cum, in! Lorem ipsum dolor sit amet, consectetur
              adipisicing elit. Magnam numquam pariatur itaque, vel quis sequi
              magni harum minus nulla molestias quibusdam veritatis corporis
              excepturi architecto non dolore nisi ratione expedita.
            </p>
            <Button />
          </div>
          <img src="@/assets/images/espelho.jpg" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.container-servicos {
  width: 100vw;
  background: #0b232e;
}
.titulo-servicos {
  text-align: center;
  font-weight: bold;
  padding-top: 60px;
}


.titulo-servicos h1 {
  font-size: 4.6rem;
  color: #309ac7;
}
.titulo-servicos h2 {
  margin-left: 280px;
  font-size: 3rem;
  color: white;
  position: relative;
}
.titulo-servicos h2::before {
  content: '';
  width: 140px;
  height: 3px;
  background: #309ac7;
  position: absolute;
  bottom: -20px;
}
.servicos-itens {
  width: 100vw;
  max-width: 1200px;
  margin: 80px auto;
}
.servicos-itens .infos-img {
  display: flex;
}
.servicos-itens .item p {
  color: white;
}
.servicos-itens .item img {
  width: 500px;
  height: 500px;
  margin-bottom: 40px;
  border: 5px solid white;
}

.info {
  margin: 100px 100px;
  color: white;
}
.info h2 {
  font-size: 2.8rem;
  position: relative;
  margin: 20px 0;
}

.info h2::before {
  content: '';
  width: 140px;
  height: 3px;
  background: #309ac7;
  position: absolute;
  bottom: 0px;
  margin-bottom: -10px;
}
</style>
