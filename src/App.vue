<template>
  <div id="app">
    <Profesionales/>
  </div>
</template>

<script>
import Profesionales from "./components/Profesionales";

export default {
  name: "App",
  components: {
    Profesionales
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
