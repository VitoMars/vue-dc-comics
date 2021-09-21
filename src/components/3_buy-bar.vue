<template>
  <div class="container-primary">
    <div class="content">
      <!-- Digital Comics -->
      <li>
        <a href="">
          <img src="@/assets/img/buy-comics-digital-comics.png" alt="" />
          Digital Comics
        </a>
      </li>
      <!-- DC Merchandise -->
      <li>
        <a href="">
          <img src="@/assets/img/buy-comics-merchandise.png" alt="" />
          DC Merchandise
        </a>
      </li>
      <!-- Subscription -->
      <li>
        <a href="">
          <img src="@/assets/img/buy-comics-subscriptions.png" alt="" />
          Subscription
        </a>
      </li>
      <!-- Comic Shop Locator -->
      <li>
        <a href="">
          <img src="@/assets/img/buy-comics-shop-locator.png" alt="" />
          Comic Shop Locator
        </a>
      </li>
      <!-- Power Visa -->
      <li>
        <a href="">
          <img src="@/assets/img/buy-dc-power-visa.svg" alt="" />
          DC Power Visa
        </a>
      </li>
    </div>
  </div>
</template>

<script>
export default {
  name: "buy-bar",
  props: {},
};
</script>

<style lang="scss" scoped>
@import "@/style/generals";
@import "@/style/mixins";
@import "@/style/colors";

.container-primary {
  background-color: $primary;
}

.content {
  @include center-content();
  @include space-between();
  @include align-center();
  flex-wrap: wrap;
  height: 200px;
  width: 100%;
  font-size: 20px;
  font-weight: bold;
  color: white;
}

li {
  @include center();
}

a {
  @include center();
  text-decoration: none;
  color: white;
  img {
    height: 70px;
    margin-right: 10px;
  }
}
</style>
