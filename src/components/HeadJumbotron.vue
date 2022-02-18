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
            <span class="pe-3"
              ><a href="#">
                {{ i.tel }}
              </a></span
            >
            <span class="pe-3">
              <a href="#">
                {{ i.email }}
              </a>
            </span>
            <span>
              <a href="#" class="pe-2">
                <i class="fa-brands fa-facebook-f"></i>
              </a>
              <a href="#" class="pe-2">
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
    <div id="jumbotron">
      <div class="container">
        <nav class="navbar navbar-expand-lg" id="personal-nav">
          <div class="container-fluid">
            <a class="navbar-brand" href="#"><span id="logo">NEXT</span>GEN</a>
            <button class="navbar-toggler" type="button">
              <span class="navbar-toggler-icon"></span>
            </button>
            <div id="navbarNav">
              <ul class="navbar-nav">
                <li class="nav-item">
                  <a class="nav-link" href="#">HOME</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link" href="#">ABOUT</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link">SERVICES</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link">PRICING</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link">BLOG</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link">GET IN TOUCH</a>
                </li>
              </ul>
            </div>
          </div>
        </nav>
      </div>
    </div>
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
  background-color: #4e4d51;
  color: #e3e7df;
  .fa-brands {
    color: #e3e7df;
  }
  a {
    color: #e3e7df;
    text-decoration: none;
  }
}

#jumbotron {
  height: 1500px;
  background-image: url(../assets/img/hero-image.png);
  background-repeat: no-repeat;
  background-size: cover;
  a {
    text-decoration: none;
    color: white;
  }
  &::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.3);
  }
}

#logo {
  color: #038483;
}
</style>