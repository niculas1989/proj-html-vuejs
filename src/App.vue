<template>
  <div>
    <!-- TODO: rivedere la centralizzazione -->
    <header>
      <HeadJumbotron :info="headerInfo" />
    </header>
    <main>
      <MainSection :title="companySection" />
    </main>
    <footer>
      <FooterPage
        :elements="footerAbout"
        :items="footerServices"
        :groups="footerSupport"
        :info="headerInfo"
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
          adress: "Main Avenue, 987",
        },
      ],
      footerAbout: [
        {
          title: "About",
          one: "The Company",
          two: "Institutuinal",
          three: "Social & Events",
          four: "Innovation",
          five: "Environment",
          six: "Technology",
        },
      ],
      footerServices: [
        {
          title: "Services",
          one: "Audit & Assurance",
          two: "Financial Advisory",
          three: "Analystics M&A",
          four: "Middle Marketing",
          five: "Legal Consulting",
          six: "Regulatory Risk",
        },
      ],
      footerSupport: [
        {
          title: "Support",
          one: "Responsability",
          two: "Terms of Use",
          three: "About Cookies",
          four: "Privacy Politicy",
          five: "Accessibility",
          six: "Information",
        },
      ],
      companySection: [
        {
          upper: "ABOUT THE NETWORK",
          bckTitle: "The",
          restOfTitle: "Company",
          paragraph:
            "For 12 years we have been providing audit and warranty, financial advice, risk advice, taxes and releted services to select clients.",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "./assets/scss/style.scss";
</style>
