<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Estam a l'any" v-bind:any="year" />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
data: function() { 
   return {
     //Aqui les meves data
     year: 2020
   }
 }
}
</script>

<style>

</style>
