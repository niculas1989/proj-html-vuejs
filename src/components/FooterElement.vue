<template>
  <div>
    <div class="square">
      <ul v-for="(e, index) in elements" :key="index">
        <li>
          <h6 class="pt-3">{{ e.title }}</h6>
        </li>
        <li class="pt-2">
          <a href="#"> > {{ e.one }} </a>
        </li>
        <li>
          <a href="#">> {{ e.two }}</a>
        </li>
        <li>
          <a href="#">> {{ e.three }}</a>
        </li>
        <li>
          <a href="#">> {{ e.four }}</a>
        </li>
        <li>
          <a href="#">> {{ e.five }}</a>
        </li>
        <li>
          <a href="#">> {{ e.six }}</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterElement",
  props: ["elements"],
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";

.square {
  height: 200px;
  background-color: $background_single_card;
  border-radius: 5px;
  a {
    color: $text_primary;
    text-decoration: none;
    &:hover {
      color: $prim_color;
    }
  }
}

ul,
li {
  list-style-type: none;
  font-size: 0.6rem;
  color: $text_primary;
  padding-bottom: 0.3rem;
  h6 {
    color: white;
  }
}
</style>