<template>
  <div>
    <div id="header-top">
      <div class="container">
        <nav class="d-flex align-items-center justify-content-between">
          <section id="left-info">PROVA</section>
          <section id="right-info">PROVA</section>
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
}
</style>