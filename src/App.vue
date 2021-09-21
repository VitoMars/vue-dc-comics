<template>
  <div id="app">
    <Header />
    <Content />
    <BuyBar />
  </div>
</template>

<script>
import Header from "./components/1_header.vue";
import Content from "./components/2_content.vue";
import BuyBar from "./components/3_buy-bar.vue";

export default {
  name: "App",
  components: {
    Header,
    Content,
    BuyBar,
  },
};
</script>

<style lang="scss">
@import "@/style/generals.scss";
@import url("https://fonts.googleapis.com/css2?family=Roboto&display=swap");
#app {
  font-family: "Roboto", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  margin-top: 30px;
}
</style>
