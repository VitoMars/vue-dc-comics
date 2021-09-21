<template>
  <div class="container-black">
    <div class="content">
      <Card
        v-for="(comic, index) in comics"
        :key="index"
        :img-url="comic.thumb"
        :text="comic.series"
      />
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

.container-black {
  background-color: black;
}

.content {
  @include center-content();
  @include align-center();
  flex-wrap: wrap;
  width: 100%;
  margin-top: 20px;
  padding: 40px 0px;
  color: white;
}
</style>
