<template>
  <div>
    <!-- Sezione in cui raccogliere info generiche sull'azienda -->
    <section id="performance-section">
      <!-- DA RIVEDERE -->
      <PerformanceCard />
    </section>

    <!-- Sezione in cui descriviamo l'azienda -->
    <section id="company">
      <CompanySection />
    </section>
  </div>
</template>

<script>
import PerformanceCard from "./PerformanceCard.vue";
import CompanySection from "./CompanySection.vue";
export default {
  components: {
    PerformanceCard,
    CompanySection,
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";
#performance-section {
  height: 400px;
  background-color: $background_first_section;
}

#company {
  height: 700px;
  max-width: 100vw;
}
</style>