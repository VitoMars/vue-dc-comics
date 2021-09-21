<template>
  <div class="container-black">
    <div class="series">Current Series</div>
    <div class="content">
      <Card
        v-for="(comic, index) in comics"
        :key="index"
        :img-url="comic.thumb"
        :text="comic.series"
      />
    </div>
    <div>
      <Button />
    </div>
  </div>
</template>

<script>
import Card from "@/components/Card.vue";
import series from "@/assets/data/dc-comics.js";
import Button from "@/components/StandardButton.vue";

export default {
  name: "content",
  props: {},
  components: {
    Card,
    Button,
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
  position: relative;
  background-color: $light-black;
  margin-top: 20px;
  padding: 40px 0px;
}

.series {
  position: absolute;
  top: -20px;
  left: 17%;
  font-size: 20px;
  padding: 10px 30px;
  color: white;
  text-transform: uppercase;
  font-weight: bold;
  background-color: $primary;
}

.content {
  @include center-content();
  @include center();
  flex-wrap: wrap;
  width: 100%;
  color: white;
}
</style>
