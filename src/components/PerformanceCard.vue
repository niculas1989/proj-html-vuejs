<template>
  <div class="container h-100 d-flex align-items-center justify-content-center">
    <div
      class="
        square
        me-5
        d-flex
        align-items-start
        justify-content-center
        ps-3
        flex-column
      "
    >
      <div class="container">
        <div class="round-bck">
          <i class="fa-solid fa-user-group pb-2 pt-2"></i>
        </div>
        <div class="pb-2 fw-bold">Human Capital</div>
        <p>
          Humanazing business: Harness the power of technology to improve the
          way people work.
        </p>
      </div>
    </div>
    <div
      class="
        square
        me-5
        d-flex
        align-items-start
        justify-content-center
        ps-3
        flex-column
      "
    >
      <!--AGGIUNGERE ICONA GIUSTA -->
      <div class="container">
        <div class="round-bck">
          <i class="fa-solid fa-chart-line"></i>
        </div>
        <div class="pb-2 fw-bold">Core Business</div>
        <p>
          It takes innovative approches to transform, modernize, and run
          existing platforms.
        </p>
      </div>
    </div>
    <div
      class="
        square
        d-flex
        align-items-start
        justify-content-center
        ps-3
        flex-column
      "
    >
      <!--AGGIUNGERE ICONA GIUSTA -->
      <div class="container">
        <div class="round-bck">
          <i class="fa-solid fa-gauge-high"></i>
        </div>
        <div class="pb-2 fw-bold">Performance</div>
        <p class="text-center">
          Achieving maximum impact and value from invesments in finance and
          supply chain.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "PerformanceCard",
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";

.round-bck {
  height: 40px;
  width: 40px;
  border-radius: 50%;
  background-color: #daeced;

  /* CENTRATURA */
  display: flex;
  justify-content: center;
  align-items: center;
}

p {
  font-size: 0.6rem;
  color: $text_primary;
}

.square {
  height: 200px;
  width: 280px;
  background-color: #fff;
  border-radius: 15px;
  &:hover {
    transform: translateY(-10px);
  }
}

i {
  color: $prim_color;
}
</style>