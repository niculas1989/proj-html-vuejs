<template>
  <div>
    <div class="container pt-5">
      <div class="col-3">
        <div class="text-center">
          <h5>NEXT GEN</h5>
          <p>A Functional HTML Template for Corporate & Business.</p>
          <div class="pb-1">
            <i class="fa-solid fa-phone"></i>
            <p class="d-inline ps-2">+1(305) 1234-5678</p>
          </div>
          <div class="pb-1">
            <i class="fa-solid fa-envelope"></i>
            <p class="d-inline ps-2">hello@example.com</p>
          </div>
          <div class="pb-3">
            <i class="fa-solid fa-location-dot"></i>
            <p class="d-inline ps-2">Main Avenue, 987</p>
          </div>
          <div id="button">
            <button class="btn btn-outline-primary">GET IN TOUCH</button>
          </div>
        </div>
      </div>
      <div class="col-3"></div>
      <div class="col-3"></div>
      <div class="col-3"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterPage",
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";

.container {
  color: white;
  button {
    border-color: $prim_color;
    color: white;
    &:hover {
      background-color: $prim_color;
      color: white;
    }
  }
}

p {
  font-size: 0.6rem;
  color: $text_primary;
}
</style>