<template>
  <div class="card">
    <div class="img-box">
      <img :src="imgUrl" :alt="text + 'thumb'" />
      <p>{{ text }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: {
    imgUrl: String,
    text: String,
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/mixins";
.img-box {
  height: 250px;
  width: 200px;
  padding: 0px 10px;
  font-size: 14px;
}
img {
  @include center();
  flex-wrap: wrap;
  height: 175px;
  width: 175px;
}
p {
  padding-top: 20px;
  text-transform: uppercase;
}
</style>
