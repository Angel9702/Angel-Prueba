<template>
<!--  -->
  <div class="card">
    <div class="card-container" v-for="(item, index) in cards" :key="index">

        <img class="img" :src="item.img" alt="imagen1">

      <div class="info">
        <div class="info-title">
          <img :src="item.icon" alt="icono">
          <span class="info-head">
            {{ item.head }}
          </span>
        </div>
        <div class="info-body">
          {{ item.body }}
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Card',
  data() {
    return {
      cards: [
        { img: require('@/assets/img1.svg'), icon: require('@/assets/1.svg'), head: 'Aqui podras encontrar...', body: 'Todo el material de tus clases , asi como los accesos directos'},
        { img: require('@/assets/img2.svg'), icon: require('@/assets/2.svg'), head: 'Aqui podras encontrar...', body: 'Nuestro club laboral, con distintas ofertas de las mejores empresas del mercado'},
        { img: require('@/assets/img3.svg'), icon: require('@/assets/3.svg'), head: 'Aqui podras encontrar...', body: 'Eventos, charlas, conferencias, voluntariados y actividades que organizamos para ti'}
      ] 
    }
  },
}
</script>

<style scoped>
.card {
  display: grid;
  grid-template-columns: repeat(1,1fr);
  gap: 1.25rem;
}
.card-container {
  background-color: white;
  padding-bottom: 1.5625rem;
  display: inline-block;
}
.info {
  padding: 0.625rem 0.9375rem;
  padding-top: 0.9375rem;
}
.info-title {
  display: flex;
  align-items: center;
}
 .info-head {
   margin-left: 10px;
   font-size: 0.875rem;
   font-weight: bold;
}
.info-body {
  margin-top: 10px;
  font-size: 0.9375rem
}
.marginIcon {
  margin-right: 0.625rem;
  color: rgb(129, 0, 250);
}
.img {
  width: 100%;
  object-fit: contain;
}
@media (min-width: 576px) { 
  .card {
    grid-template-columns: repeat(2,1fr);
  }
 }
 /* Medium devices (tablets, 768px and up) */
@media (min-width: 768px) { 
  .card {
    grid-template-columns: repeat(2,1fr);
  }
 }
/* Large devices (desktops, 992px and up) */
@media (min-width: 992px) { 
  .card {
    grid-template-columns: repeat(3,1fr);
  }
 }
 /* Extra large devices (large desktops, 1200px and up) */
@media (min-width: 1200px) { 
  .card {
    grid-template-columns: repeat(3,1fr);
  }
 }
</style>