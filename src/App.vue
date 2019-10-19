<template>
  <div id="app">
    <h1>Open Green House</h1>
    <AddPlant/>
  </div>
</template>

<script>
import AddPlant from './components/AddPlant.vue'

export default {
  name: 'app',
  components: {
    AddPlant
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 60px auto ;
  width: 75%;

}
</style>
