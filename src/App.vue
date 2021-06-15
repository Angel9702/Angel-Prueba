<template>
  <div id="app">
    <header-component />
    <main class="container">
    <router-view />
    </main>
  </div>
</template>
<script>
import HeaderComponent from './components/HeaderComponente.vue'
export default {
  components: {
    HeaderComponent
  }
}
</script>
<style scoped>
  .container {
    max-width: 1200px;
    width: 80%;
    margin-left: auto;
    margin-right: auto;
  }
</style>
