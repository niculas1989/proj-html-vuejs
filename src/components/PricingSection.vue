<template>
  <div class="container">
    <!-- info sui prezzi -->
    <div class="text-center pt-5">
      <div class="container-md">
        <span class="over-the-title">MONTHLY PLANS</span>
        <h2>
          <div class="bck-prim d-inline"><strong>Pricing</strong></div>
          Table
        </h2>
        <p>
          We can help you deliver and execute your future, wherever you compete,
          using the latest<br />
          technologies, from strategy development to implementation.
        </p>
      </div>
    </div>

    <!-- schede con i prezzi -->
    <div class="pt-3">
      <div class="row">
        <div class="col-4">
          <div class="card container position-relative">
            <div class="hover-arrow">
              <a href="#">
                <i class="fa-solid fa-arrow-right"></i>
              </a>
            </div>
            <div class="text-center">
              <i class="fa-solid fa-rocket pt-3"></i>
              <div><strong>Standard</strong></div>
              <div class="price fw-bolder">$490/<em>mo</em></div>
            </div>
            <ul v-for="(i, index) in item" :key="index" class="container">
              <li class="d-flex justify-content-between p-2">
                {{ i.standard }} <i class="fa-solid fa-check"></i>
              </li>

              <li class="d-flex justify-content-between p-2">
                {{ i.platform }} <i class="fa-solid fa-check"></i>
              </li>
              <li class="d-flex justify-content-between p-2">
                {{ i.business }} <i class="fa-solid fa-xmark"></i>
              </li>
              <li class="d-flex justify-content-between p-2">
                {{ i.dedicated }} <i class="fa-solid fa-xmark"></i>
              </li>
              <li class="d-flex justify-content-between p-2">
                {{ i.personal }} <i class="fa-solid fa-xmark"></i>
              </li>
            </ul>
          </div>
        </div>
        <div class="col-4">
          <div class="card container position-relative">
            <div class="badge rounded-pill">
              Most<br />
              Popular
            </div>
            <div class="hover-arrow">
              <a href="#">
                <i class="fa-solid fa-arrow-right"></i>
              </a>
            </div>
            <div class="text-center">
              <i class="fa-solid fa-briefcase pt-5"></i>
              <div><strong>Professional</strong></div>
              <div class="price fw-bolder">$890/<em>mo</em></div>
            </div>
            <ul v-for="(i, index) in item" :key="index" class="container">
              <li class="d-flex justify-content-between p-2">
                {{ i.standard }} <i class="fa-solid fa-check"></i>
              </li>

              <li class="d-flex justify-content-between p-2">
                {{ i.platform }} <i class="fa-solid fa-check"></i>
              </li>
              <li class="d-flex justify-content-between p-2">
                {{ i.business }} <i class="fa-solid fa-check"></i>
              </li>
              <li class="d-flex justify-content-between p-2">
                {{ i.dedicated }} <i class="fa-solid fa-xmark"></i>
              </li>
              <li class="d-flex justify-content-between p-2">
                {{ i.personal }} <i class="fa-solid fa-xmark"></i>
              </li>
            </ul>
          </div>
        </div>
        <div class="col-4">
          <div class="card container position-relative">
            <div class="hover-arrow">
              <a href="#">
                <i class="fa-solid fa-arrow-right"></i>
              </a>
            </div>
            <div class="text-center">
              <i class="fa-regular fa-gem pt-3"></i>
              <div><strong>Ultimate</strong></div>
              <div class="price fw-bolder">$1.390/<em>mo</em></div>
            </div>
            <ul v-for="(i, index) in item" :key="index" class="container">
              <li class="d-flex justify-content-between p-2">
                {{ i.standard }} <i class="fa-solid fa-check"></i>
              </li>

              <li class="d-flex justify-content-between p-2">
                {{ i.platform }} <i class="fa-solid fa-check"></i>
              </li>
              <li class="d-flex justify-content-between p-2">
                {{ i.business }} <i class="fa-solid fa-check"></i>
              </li>
              <li class="d-flex justify-content-between p-2">
                {{ i.dedicated }} <i class="fa-solid fa-check"></i>
              </li>
              <li class="d-flex justify-content-between p-2">
                {{ i.personal }} <i class="fa-solid fa-check"></i>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "PricingSection",
  props: ["item"],
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";

.container {
  overflow: hidden;
  .badge {
    background-color: $water_green;
    width: 80px;
    font-size: 0.6rem;

    position: absolute;
    top: 10px;
    left: -10px;
  }
  .card {
    width: 350px;
  }
}

.card:hover {
  .hover-arrow {
    display: block;
  }
}

.hover-arrow {
  position: absolute;
  top: 10px;
  right: 15px;
  display: none;
  i {
    font-size: bolder;
  }
}

.row {
  .card {
    border-radius: 10px;
  }
}

.over-the-title {
  color: $water_green;
  font-size: 0.8rem;
  font-weight: 700;
}

.bck-prim {
  color: $prim_color;
  height: 25px;
  width: 40px;
  background-color: #cce3de;
  border-radius: 3px;
}

p {
  font-size: 0.6rem;
  color: $text_primary;
}

.price,
i {
  color: $prim_color;
}

li {
  list-style-type: none;
  font-size: 0.6rem;
  color: $text_primary;
}
</style>