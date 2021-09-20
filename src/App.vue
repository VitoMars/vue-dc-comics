<template>
  <div id="app">
    <Header />
    <Links />
  </div>
</template>

<script>
import Header from "./components/header.vue";
import Links from "./assets/data/Links.js";

export default {
  name: "App",
  components: {
    Header,
    Links,
  },
};
</script>

<style lang="scss">
#app {
  @import url("https://fonts.googleapis.com/css2?family=Roboto&display=swap");
  font-family: "Roboto", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 30px;
}
</style>
