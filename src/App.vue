<template>
  <div id="app">
    <Header />
    <Links />
    <Content />
    <BuyBar />
  </div>
</template>

<script>
import Header from "./components/header.vue";
import Links from "./assets/data/Links.js";
import Content from "./components/content.vue";
import BuyBar from "./components/buy-bar.vue";

export default {
  name: "App",
  components: {
    Header,
    Links,
    Content,
    BuyBar,
  },
};
</script>

<style lang="scss">
#app {
  @import url("https://fonts.googleapis.com/css2?family=Roboto&display=swap");
  font-family: "Roboto", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  margin-top: 30px;
}
</style>
