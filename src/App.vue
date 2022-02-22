<template>
  <div>
    <header>
      <HeadJumbotron :info="headerInfo" />
    </header>
    <main>
      <MainSection />
    </main>
    <footer>
      <FooterPage
        :elements="footerAbout"
        :items="footerServices"
        :groups="footerSupport"
      />
    </footer>
  </div>
</template>

<script>
import HeadJumbotron from "./components/HeadJumbotron.vue";
import MainSection from "./components/MainSection.vue";
import FooterPage from "./components/FooterPage.vue";

export default {
  name: "App",
  components: {
    HeadJumbotron,
    MainSection,
    FooterPage,
  },
  data() {
    return {
      headerInfo: [
        {
          open: "Mon-Sat-9:00-18:00",
          tel: "+1(305) 1234-5678",
          email: "hello@example.com",
        },
      ],
      footerAbout: [
        {
          title: "About",
          company: "The Company",
          institute: "Institutuinal",
          social: "Social & Events",
          innovation: "Innovation",
          environment: "Environment",
          technology: "Technology",
        },
      ],
      footerServices: [
        {
          title: "Services",
          audit: "Audit & Assurance",
          financial: "Financial Advisory",
          analysis: "Analystics M&A",
          marketing: "Middle Marketing",
          consulting: "Legal Consulting",
          risks: "Regulatory Risk",
        },
      ],
      footerSupport: [
        {
          title: "Support",
          responsability: "Responsability",
          terms: "Terms of Use",
          cookies: "About Cookies",
          politicy: "Privacy Politicy",
          accassibility: "Accessibility",
          info: "Information",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "./assets/scss/style.scss";
</style>
