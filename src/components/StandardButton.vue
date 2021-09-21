<template>
  <div class="button">
    <button class="standardButton">Load More</button>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
@import "@/style/mixins";
@import "@/style/colors";
.button {
  @include center();
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
