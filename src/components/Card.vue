<template>
  <div class="card">
    <div class="img-box">
      <div
        class="img"
        :style="{ 'background-image': 'url(' + imgUrl + ')' }"
      ></div>
      <!-- <img :src="imgUrl" /> -->
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
  cursor: pointer;
}
.img {
  height: 175px;
  width: 175px;
  background-size: cover;
  background-position: center top;
}
img {
  height: 175px;
  width: 175px;
  //   background-size: cover;
  //   background-position: center top;
}
p {
  padding-top: 20px;
  text-transform: uppercase;
}
</style>
