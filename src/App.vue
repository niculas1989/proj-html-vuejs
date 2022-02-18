<template>
  <div>
    <header>
      <HeadJumbotron :info="headerInfo" />
    </header>
    <main>
      <MainSection />
    </main>
    <footer>
      <FooterPage />
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
    };
  },
};
</script>

<style lang="scss">
@import "./assets/scss/style.scss";
</style>
