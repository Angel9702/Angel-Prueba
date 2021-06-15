<template>
  <div class="home">
    <h1>Conoce los beneficios de EVA, tu entorno Virtual de Trabajo</h1>
    <card-component />
     <div class="button-container">
      <button class="button">Comenzar</button>
    </div>
  </div>
</template>

<script>
import CardComponent from '../components/CardComponent.vue'

export default {
  name: 'Home',
  components: {
    CardComponent
  }
}
</script>
<style scoped>
h1 {
  text-align: center;
}
.button-container {
  display: flex;
  justify-content: center;
  margin-bottom: 1.25rem;
  margin-top: 1.25rem;
}
.button {
  background-color: blueviolet;
  border-radius: 0.375rem;
  padding: 0.875rem 15px;
  width: 100%;
  border: none;
  color: white;
  text-align: center;
}
@media (min-width: 576px) {
 }
 /* Medium devices (tablets, 768px and up) */
@media (min-width: 768px) { 
  h1 {
    font-size: 2rem;
  }
}
/* Large devices (desktops, 992px and up) */
@media (min-width: 992px) {  
.button-container {
  display: flex;
  justify-content: flex-end;
  margin-bottom: 1.25rem;
  margin-top: 1.25rem;
}
.button {
  width: 200px;
}
}
 /* Extra large devices (large desktops, 1200px and up) */
@media (min-width: 1200px) { }
</style>