<template>
  <div>
    <section id="performance-section">
      <div
        class="container h-100 d-flex align-items-center justify-content-around"
      >
        <div
          class="square me-2 d-flex align-items-center justify-content-center"
        >
          contenuto
        </div>
        <div
          class="square me-2 d-flex align-items-center justify-content-center"
        >
          contenuto
        </div>
        <div class="square d-flex align-items-center justify-content-center">
          contenuto
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";

#performance-section {
  height: 240px;
  background-color: $background_first_section;
}

.square {
  height: 130px;
  width: 180px;
  background-color: #fff;
}
</style>