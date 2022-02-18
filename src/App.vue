<template>
  <div>
    <header>
      <Jumbotron />
    </header>
    <main>
      <Main />
    </main>
    <footer>
      <Footer />
    </footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
  data() {
    return {
      headerInfo: {
        open: "Mon-Sat-9:00-18:00",
        tel: "+1(305) 1234-5678",
        email: "hello@example.com",
      },
    };
  },
};
</script>

<style lang="scss">
@import "./assets/scss/style.scss";
</style>
