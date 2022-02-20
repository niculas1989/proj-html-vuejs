<template>
  <div>
    <div class="container pt-5">
      <div class="row">
        <div class="col-3">
          <div class="text-center">
            <h5><span class="bck-prim">NEXT</span> GEN</h5>
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

        <!-- TODO ragionare sul creare delle carte -->
        <div class="col-3">
          <div class="square">
            <ul>
              <li>
                <h6 class="pt-3">About</h6>
              </li>
              <li class="pt-2">> The Company</li>
              <li>> Insitutional</li>
              <li>> Social & Events</li>
              <li>> Innovation</li>
              <li>> Environment</li>
              <li>> Technology</li>
            </ul>
          </div>
        </div>
        <div class="col-3">
          <div class="square">
            <ul>
              <li>
                <h6 class="pt-3">About</h6>
              </li>
              <li class="pt-2">> The Company</li>
              <li>> Insitutional</li>
              <li>> Social & Events</li>
              <li>> Innovation</li>
              <li>> Environment</li>
              <li>> Technology</li>
            </ul>
          </div>
        </div>
        <div class="col-3">
          <div class="square">
            <ul>
              <li>
                <h6 class="pt-3">About</h6>
              </li>
              <li class="pt-2">> The Company</li>
              <li>> Insitutional</li>
              <li>> Social & Events</li>
              <li>> Innovation</li>
              <li>> Environment</li>
              <li>> Technology</li>
            </ul>
          </div>
        </div>
      </div>
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

.square {
  height: 200px;
  background-color: $background_single_card;
  border-radius: 5px;
}

.bck-prim {
  color: $water_green;
  height: 20px;
  width: 30px;
  background-color: $water_green;
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