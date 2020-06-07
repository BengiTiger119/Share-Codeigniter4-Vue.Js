<template>
  <div id="app">
    <img alt="Ci logo" src="./assets/ci.png" height="64" />
    &nbsp;&nbsp;
    <img alt="Vue logo" src="./assets/logo-52x52.png" />
    <HelloWorld msg="Cli 4.4.1" site="CiKorea.net" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 20px;
}
</style>
