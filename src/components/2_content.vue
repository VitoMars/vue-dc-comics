<template>
  <div class="container-black">
    <div class="content">--> Content goes here</div>
  </div>
</template>

<script>
export default {
  name: "content",
  props: {},
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
  height: 200px;
  width: 100%;
  margin-top: 20px;
  font-size: 25px;
  font-weight: bold;
  color: white;
}
</style>
