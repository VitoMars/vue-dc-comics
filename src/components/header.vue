<template>
  <div class="header">
    <img src="@/assets/img/dc-logo.png" alt="" />
    <div class="links">
      <ul>
        <li v-for="(link, index) in links" :key="index">
          <a href="link.url">
            {{ link.text }}
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
import { headerLinks } from "../assets/data/Links";
export default {
  name: "header",
  props: {},
  data() {
    return {
      links: headerLinks,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/style/mixins";

.header {
  @include space-around();
}

h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;

  text-transform: uppercase;
}
a {
  text-decoration: none;
  color: #303030;
  font-weight: bold;
}
</style>
