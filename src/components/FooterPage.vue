<template>
  <div id="footer-page" class="d-flex flex-column justify-content-between">
    <div class="container pt-5">
      <div class="row">
        <div class="col-3" v-for="(element, index) in info" :key="index">
          <div class="text-center">
            <h5><span class="bck-prim">NEXT</span> GEN</h5>
            <p>A Functional HTML Template for Corporate & Business.</p>
            <div class="pb-1">
              <i class="fa-solid fa-phone"></i>
              <p class="d-inline ps-2">{{ element.tel }}</p>
            </div>
            <div class="pb-1">
              <i class="fa-solid fa-envelope"></i>
              <p class="d-inline ps-2">{{ element.email }}</p>
            </div>
            <div class="pb-3">
              <i class="fa-solid fa-location-dot"></i>
              <p class="d-inline ps-2">{{ element.adress }}</p>
            </div>
            <div id="button">
              <button class="btn btn-outline-primary">GET IN TOUCH</button>
            </div>
          </div>
        </div>

        <div class="col-3">
          <FooterElement :elements="elements" />
        </div>
        <div class="col-3">
          <FooterElement :elements="items" />
        </div>
        <div class="col-3">
          <FooterElement :elements="groups" />
        </div>
      </div>
    </div>
    <div id="bottom-footer" class="position-relative">
      <a href="up">
        <div class="arrow-up">
          <i class="fa-solid fa-arrow-up"></i>
        </div>
      </a>
      <div class="container h-100">
        <div class="d-flex justify-content-between align-items-center h-100">
          <span
            >Enjoy the low price. We are tracking any intention of piracy</span
          >
          <span>
            <i class="fa-regular fa-copyright"></i>
            2022 NEXGEN is Proudly Powered by
            <span id="proud">Boolean</span> Student with
            <i class="fa-solid fa-heart"></i>
          </span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import FooterElement from "./FooterElement.vue";
export default {
  name: "FooterPage",
  props: ["elements", "items", "groups", "info"],
  components: { FooterElement },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";

.arrow-up {
  position: absolute;
  right: 15px;
  top: 12px;
  height: 30px;
  width: 30px;
  background-color: #19191c;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
}
a {
  color: #000;
  &:hover {
    transform: translateY(-10px);
    color: $prim_color;
  }
}

#footer-page {
  height: 350px;
  background-color: $background_dark;
  #bottom-footer {
    height: 50px;
    background-color: #000;
    span {
      font-size: 0.6rem;
      color: $text_primary;
    }
    .fa-heart {
      color: darkred;
    }
    #proud {
      color: $prim_color;
    }
  }
}

.bck-prim {
  color: $water_green;
  height: 20px;
  width: 30px;
  background-color: #0e272d;
  border-radius: 3px;
}

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