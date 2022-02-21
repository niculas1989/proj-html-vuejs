<template>
  <div>
    <!-- Sezione in cui raccogliere info generiche sull'azienda -->
    <div id="performance-section">
      <!-- DA RIVEDERE -->
      <PerformanceCard />
    </div>

    <!-- Sezione in cui descriviamo l'azienda -->
    <div id="company">
      <!-- DA RIVEDERE -->
      <CompanySection />
    </div>

    <!-- Sezione in cui descriviamo le eccellenze dell'azienda -->
    <div id="excellence">
      <!-- DA RIVEDERE -->
      <ExcellenceSection />
    </div>

    <!-- Sezione in cui descriviamo le eccellenze dell'azienda -->
    <div id="pricing">
      <!-- DA RIVEDERE -->
      <PricingSection :item="price" />
    </div>

    <!-- Sezione in cui descriviamo le ultime novità dell'azienda -->
    <div id="news">
      <!-- DA RIVEDERE anche le funzioni HOVER-->
      <LatestNews />
    </div>

    <div id="newsletter" class="pt-5">
      <!-- DA RIVEDERE -->
      <NewsletterSection />
    </div>

    <div id="mailsection">
      <!-- DA RIVEDERE -->
      <MailSection />
    </div>
  </div>
</template>

<script>
import PerformanceCard from "./PerformanceCard.vue";
import CompanySection from "./CompanySection.vue";
import ExcellenceSection from "./ExcellenceSection.vue";
import PricingSection from "./PricingSection.vue";
import LatestNews from "./LatestNews.vue";
import NewsletterSection from "./NewsletterSection.vue";
import MailSection from "./MailSection.vue";

export default {
  name: "MainSection",
  components: {
    PerformanceCard,
    CompanySection,
    ExcellenceSection,
    PricingSection,
    LatestNews,
    NewsletterSection,
    MailSection,
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

#newsletter {
  height: 300px;
}

#performance-section {
  height: 400px;
  background-color: $background_first_section;
}

#company {
  height: 800px;
  /* max-width: 100vw; */
  overflow: hidden;
}

#excellence {
  height: 700px;
  background-color: $background_dark;
  color: white;
}

#pricing {
  height: 500px;
  background-color: $background_first_section;
}
</style>