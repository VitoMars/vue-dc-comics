<template>
  <div class="content">--> Content goes here</div>
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
.content {
  @include align-center();
  height: 200px;
  width: 100%;
  margin-top: 20px;
  font-size: 25px;
  font-weight: bold;
  color: white;
  background-color: black;
  padding: 0px 200px;
}
</style>
