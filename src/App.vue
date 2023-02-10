<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld />
  <manga />
  <div></div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import manga from './components/manga.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    manga
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
*{
  padding : 0;
  margin : 0;
  list-style: none;
}
</style>
