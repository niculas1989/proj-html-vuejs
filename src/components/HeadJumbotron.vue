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
    <div class="position-relative">
      <div id="jumbotron">
        <div class="container h-100">
          <nav class="navbar navbar-expand-lg" id="personal-nav">
            <div class="container-fluid">
              <a class="navbar-brand" href="#"
                ><span id="logo" class="bck-prim">NEXT</span>GEN</a
              >
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
          <div
            id="lead-customer"
            class="
              d-flex
              align-items-center
              justify-content-center
              h-100
              flex-column
            "
          >
            <section class="text-center">
              <h1 id="title">Lead ~ Customer</h1>
              <p>
                Successful strategies require data analysis, creativity and
                customer focus, taking advantage of the best and latest
                technologies to offer excellent services.
              </p>
            </section>
            <section>
              <button id="first-btn" type="button" class="btn btn me-3">
                GET IN TOUCH
              </button>
              <button id="second-btn" type="button" class="btn btn-outline">
                READ MORE
              </button>
            </section>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderJumbotron",
  props: ["info"],
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";
.bck-prim {
  color: $water_green;
  height: 20px;
  width: 30px;
  background-color: $water_green;
  border-radius: 3px;
  opacity: 0.5;
}

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
  height: 700px;
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
    url(../assets/img/hero-image.png);
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  #title {
    font-weight: 800;
  }
}

#personal-nav {
  font-weight: 600;
  height: 50px;
}
a {
  text-decoration: none;
  color: white;
}

#lead-customer {
  color: white;
}

#first-btn {
  background-color: $prim_color;
  color: white;
}

#second-btn {
  border-color: $prim_color;
  color: white;
  &:hover {
    background-color: $prim_color;
  }
}

#logo {
  color: $prim_color;
}
</style>