<template>
  <div>
    <div id="header-top">
      <div class="container h-100">
        <nav
          v-for="(i, index) in info"
          :key="index"
          class="d-flex align-items-center justify-content-between h-100"
        >
          <section id="left-info">
            <span>
              <i class="fa-solid fa-clock"></i>
              Open Hours: {{ i.open }}</span
            >
          </section>
          <section id="right-info">
            <span>{{ i.tel }}</span>
            <span>{{ i.email }}</span>
            <span>
              <a href="#">
                <i class="fa-brands fa-facebook-f"></i>
              </a>
              <a href="#">
                <i class="fa-brands fa-twitter"></i>
              </a>
              <a href="#">
                <i class="fa-brands fa-linkedin-in"></i>
              </a>
            </span>
          </section>
        </nav>
      </div>
    </div>
    <div id="jumbotron"></div>
  </div>
</template>

<script>
export default {
  props: ["info"],
};
</script>

<style scoped lang="scss">
#header-top {
  height: 50px;
  background-color: #778a94;
  color: #e3e7df;
  .fa-brands {
    color: #e3e7df;
  }
}
</style>