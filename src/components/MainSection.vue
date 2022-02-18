<template>
  <div>
    <!-- Sezione in cui raccogliere info generiche sull'azienda -->
    <section id="performance-section">
      <!-- DA RIVEDERE -->
      <PerformanceCard />
    </section>

    <!-- Sezione in cui descriviamo l'azienda -->
    <section id="company">
      <!-- DA RIVEDERE -->
      <CompanySection />
    </section>

    <!-- Sezione in cui descriviamo le eccellenze dell'azienda -->
    <section id="excellence">
      <!-- DA RIVEDERE -->
      <ExcellenceSection />
    </section>
  </div>
</template>

<script>
import PerformanceCard from "./PerformanceCard.vue";
import CompanySection from "./CompanySection.vue";
import ExcellenceSection from "./ExcellenceSection.vue";
export default {
  components: {
    PerformanceCard,
    CompanySection,
    ExcellenceSection,
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

#excellence {
  height: 700px;
  background-color: #121117;
  color: white;
}
</style>