<template>
  <div>
    <div
      class="container pt-4"
      v-for="(element, index) in excellenceTitle"
      :key="index"
    >
      <span class="over-the-title">{{ element.upper }}</span>
      <h2>
        {{ element.restOfTitle }}
        <span class="bck-prim">{{ element.bckTitle }}</span>
      </h2>
      <div class="row">
        <div class="col-10">
          <p>
            {{ element.paragraph }}
          </p>
        </div>
        <div class="col-2">
          <button type="button" class="btn btn-outline">SEE ALL</button>
        </div>
      </div>

      <!-- 6 quadrati che racchiudono le eccellenze dell'azienda -->

      <div class="row pt-3 g-4">
        <div class="col-4">
          <div class="square">
            <div class="container">
              <i class="fa-solid fa-network-wired pt-3"></i>
              <div class="fw-bold">Audit & Assurance</div>
              <div>
                <p class="pt-2 pb-3">
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                </p>
              </div>
              <button type="button" class="btn btn-outline">READ MORE</button>
            </div>
          </div>
        </div>
        <div class="col-4">
          <div class="square">
            <div class="container">
              <i class="fa-solid fa-briefcase pt-3"></i>
              <div class="fw-bold">Financial Advisory</div>
              <div>
                <p class="pt-2 pb-3">
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                </p>
              </div>
              <button type="button" class="btn btn-outline">READ MORE</button>
            </div>
          </div>
        </div>
        <div class="col-4">
          <div class="square">
            <div class="container">
              <i class="fa-solid fa-chart-line pt-3"></i>
              <div class="fw-bold">Analytics and M&A</div>
              <div>
                <p class="pt-2 pb-3">
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                </p>
              </div>

              <button type="button" class="btn btn-outline">READ MORE</button>
            </div>
          </div>
        </div>
        <div class="col-4">
          <div class="square">
            <div class="container">
              <i class="fa-solid fa-plane-departure pt-3"></i>
              <div class="fw-bold">Middle Marketing</div>
              <div>
                <p class="pt-2 pb-3">
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                </p>
              </div>
              <button type="button" class="btn btn-outline">READ MORE</button>
            </div>
          </div>
        </div>
        <div class="col-4">
          <div class="square">
            <div class="container">
              <i class="fa-solid fa-earth-europe pt-3"></i>
              <div class="fw-bold">Legal Consulting</div>
              <div>
                <p class="pt-2 pb-3">
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                </p>
              </div>
              <button type="button" class="btn btn-outline">READ MORE</button>
            </div>
          </div>
        </div>
        <div class="col-4">
          <div class="square">
            <div class="container">
              <i class="fa-solid fa-box-open pt-3"></i>
              <div class="fw-bold">Regularoty Risk</div>
              <div>
                <p class="pt-2 pb-3">
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                </p>
              </div>
              <button type="button" class="btn btn-outline">READ MORE</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ExcellenceSection",
  data() {
    return {
      excellenceTitle: [
        {
          upper: "OUR BUSINESS AREAS",
          bckTitle: "Services",
          restOfTitle: "Excellence in",
          paragraph:
            "We are leaders in providing consultancy with a set of cutting-edge technologies and a team of experienced and renowned professionals. These are some options that you can hire.",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";
.bck-prim {
  color: #fff;
  height: 25px;
  width: 45px;
  background-color: #0e272d;
  border-radius: 3px;
  opacity: 1;
}

button {
  border-color: $prim_color;
  color: white;
  &:hover {
    background-color: $prim_color;
    color: white;
  }
}

.over-the-title {
  color: $prim_color;
  font-size: 0.8rem;
  font-weight: 700;
}

.square {
  height: 200px;
  width: 350px;
  background-color: $background_single_card;
  border-radius: 5px;
  i {
    color: $prim_color;
  }
}

.square:hover {
  i,
  p {
    color: #fff;
  }
}

p {
  font-size: 0.6rem;
  color: $text_primary;
}
</style>