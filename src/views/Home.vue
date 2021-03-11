<template>
  <div class="home">
    <img alt="logoG" src="../assets/Mortel-modifier.png">
    <HelloWorld msg="Bienvenue sur le site de Geronde"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>

<style>
img {
  width: 20%;
  height: auto;
}
</style>
