<template>
  <div class="row h-100">
    <div class="col-4 offset-2 h-100">
      <div class="d-flex flex-column justify-content-center h-100">
        <span class="over-the-title">ABOUT THE NETWORK</span>
        <h2 class="fw-bolder"><span class="bck-prim">The</span> Company</h2>
        <span
          >For 12 years we have been providing audit and warranty, financial
          advice, risk advice, taxes and releted services to select
          clients.</span
        >
        <div class="row pt-3">
          <div class="col-6">
            <i class="fa-solid fa-award pb-3"></i>
            <span class="fw-bold"> Tradition </span>
            <div>
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
            </div>
          </div>
          <div class="col-6">
            <i class="fa-solid fa-lock"></i>
            <span class="fw-bold"> Security </span>
            <div>
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
            </div>
          </div>
          <div class="col-6">
            <i class="fa-solid fa-certificate"></i>
            <span class="fw-bold"> Certificate </span>
            <div>
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
            </div>
          </div>
          <div class="col-6">
            <i class="fa-solid fa-graduation-cap"></i>
            <span class="fw-bold"> Expertise </span>
            <div>
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="col-6">
      <img
        src="../assets/img/about-3.jpg"
        alt="Man with coffe working"
        class="img-fluid"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: "CompanySection",
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";

img {
  height: 100%;
  width: 100%;
  overflow: hidden;
}

.bck-prim {
  color: $prim_color;
  height: 20px;
  width: 30px;
  background-color: #daeced;
  border-radius: 3px;
}

p {
  font-size: 0.6rem;
  color: $text_primary;
}

#colored {
  color: $prim_color;
}

.over-the-title {
  color: $water_green;
  font-weight: 800;
  font-size: 0.8rem;
}

i {
  color: $prim_color;
}
</style>