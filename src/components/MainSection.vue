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

    <!-- Sezione in cui descriviamo le eccellenze dell'azienda -->
    <section id="pricing">
      <!-- DA RIVEDERE -->
      <PricingSection :item="price" />
    </section>
  </div>
</template>

<script>
import PerformanceCard from "./PerformanceCard.vue";
import CompanySection from "./CompanySection.vue";
import ExcellenceSection from "./ExcellenceSection.vue";
import PricingSection from "./PricingSection.vue";

export default {
  name: "MainSection",
  components: {
    PerformanceCard,
    CompanySection,
    ExcellenceSection,
    PricingSection,
  },
  data() {
    return {
      price: [
        {
          standard: "Standard Accounting",
          platform: "Platform Access",
          business: "Business Orientation",
          dedicated: "Dedicated Consulent",
          personal: "Personal Assistance",
        },
      ],
    };
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

#pricing {
  height: 700px;
  background-color: $background_first_section;
}
</style>