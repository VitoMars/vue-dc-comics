<template>
  <div class="container-black">
    <div class="content">
      <div class="box-primary">Current Series</div>
      <Card
        v-for="(comic, index) in comics"
        :key="index"
        :img-url="comic.thumb"
        :text="comic.series"
      />
      <button class="standardButton">Load More</button>
    </div>
  </div>
</template>

<script>
import Card from "@/components/Card.vue";
import series from "@/assets/data/dc-comics.js";

export default {
  name: "content",
  props: {},
  components: {
    Card,
  },
  data() {
    return {
      comics: series,
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/generals";
@import "@/style/mixins";
@import "@/style/colors";

.container-black {
  background-color: $light-black;
  margin-top: 20px;
  padding: 40px 0px;
}

.content {
  position: relative;
  @include center-content();
  @include center();
  flex-wrap: wrap;
  width: 100%;
  color: white;
}

.box-primary {
  position: absolute;
  top: -60px;
  left: 0;
  font-size: 20px;
  padding: 10px 30px;
  color: white;
  text-transform: uppercase;
  font-weight: bold;
  background-color: $primary;
}

.standardButton {
  width: 200px;
  background-color: $primary;
  color: white;
  font-weight: bold;
  padding: 10px;
  border: none;
  text-transform: uppercase;
  cursor: pointer;
}
</style>
