<template>
  <div>
    <section id="performance-section">
      <!-- DA RIVEDERE -->
      <PerformanceCard />
    </section>
  </div>
</template>

<script>
import PerformanceCard from "./PerformanceCard.vue";
export default {
  components: {
    PerformanceCard,
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";
#performance-section {
  height: 400px;
  background-color: $background_first_section;
}
</style>