<template>
  <div class="w-100">
    <!-- <div v-for="(e, index) in item" :key="index">
      <figure>
        <p>{{ e.title }}</p>
        <img :src="require(`../assets/img/${e.img}`)" :alt="e.alt" />
      </figure>
    </div> -->
    <div class="d-flex justify-content-between pt-4 pb-5 w-100">
      <div class="squared">
        <div
          id="first-square"
          class="d-flex align-items-end position-relative h-100"
          @mouseenter="hover = true"
        >
          <div
            class="
              hover-option
              container
              pt-5
              d-flex
              flex-column
              justify-content-around
              h-100
            "
            v-if="hover"
            @mouseleave="hover = false"
          >
            <div class="d-flex justify-content-around">
              <div class="d-flex">
                <i class="fa-regular fa-user"></i>
                <p class="ps-2">Andrea Miller</p>
              </div>
              <div class="d-flex">
                <i class="fa-regular fa-clock"></i>
                <p class="ps-2">2 Days Ago</p>
              </div>
            </div>

            <div class="text-center d-flex flex-column">
              <p class="fs-3">
                <strong>Increasing creativity is possible for everyone</strong>
              </p>
              <span
                >Lorem ipsum dolor sit amet,<br />
                consectetur adipiscing elit.</span
              >
            </div>
          </div>
          <div class="d-flex justify-content-center w-100" v-else>
            <p>Increasing creativity is possible for everyone</p>
          </div>
        </div>
      </div>
      <div class="squared text-center">
        <div
          id="second-square"
          class="d-flex align-items-end position-relative h-100"
          @mouseenter="hoverSecond = true"
        >
          <div
            class="
              hover-option
              container
              pt-5
              d-flex
              flex-column
              justify-content-around
              h-100
            "
            @mouseleave="hoverSecond = false"
            v-if="hoverSecond"
          >
            <div class="d-flex justify-content-around">
              <div class="d-flex">
                <i class="fa-regular fa-user"></i>
                <p class="ps-2">Andrea Miller</p>
              </div>
              <div class="d-flex">
                <i class="fa-regular fa-clock"></i>
                <p class="ps-2">2 Days Ago</p>
              </div>
            </div>

            <div class="text-center d-flex flex-column">
              <p class="fs-3">
                <strong
                  >Because market research is part of the business plan</strong
                >
              </p>
              <span
                >Lorem ipsum dolor sit amet,<br />
                consectetur adipiscing elit.</span
              >
            </div>
          </div>
          <div class="d-flex justify-content-center w-100" v-else>
            <p>
              Because market research is part of the business planible for
              everyone
            </p>
          </div>
        </div>
      </div>
      <div class="squared">
        <div
          id="third-square"
          class="d-flex align-items-end position-relative h-100"
          @mouseenter="hoverThird = true"
        >
          <div
            class="
              hover-option
              container
              pt-5
              d-flex
              flex-column
              justify-content-around
              h-100
            "
            @mouseleave="hoverThird = false"
            v-if="hoverThird"
          >
            <div class="d-flex justify-content-around">
              <div class="d-flex">
                <i class="fa-regular fa-user"></i>
                <p class="ps-2">Andrea Miller</p>
              </div>
              <div class="d-flex">
                <i class="fa-regular fa-clock"></i>
                <p class="ps-2">2 Days Ago</p>
              </div>
            </div>

            <div class="text-center d-flex flex-column">
              <p class="fs-3">
                <strong>Working from home is now a trend</strong>
              </p>
              <span
                >Lorem ipsum dolor sit amet,<br />
                consectetur adipiscing elit.</span
              >
            </div>
          </div>
          <div class="d-flex justify-content-center w-100" v-else>
            <p>Working from home is now a trend</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "GenerateCards",
  props: ["item"],
  data() {
    return {
      hover: false,
      hoverSecond: false,
      hoverThird: false,
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";

.hover-option {
  position: absolute;
  z-index: 1;
  top: 0;
  right: 0;
  left: 0;
  bottom: 0;
  background-color: rgba(0, 0, 0, 0.4);
  border-radius: 15px;
  color: #fff;
}

.squared {
  height: 350px;
  width: 350px;
  p {
    color: white;
    font-size: 0.9rem;
    font-weight: 500;
  }
}

#first-square {
  background-image: linear-gradient(rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.3)),
    url(../assets/img/news-1.jpg);
  height: 100%;
  background-repeat: no-repeat;
  background-size: cover;
  border-radius: 15px;
  text-align: center;
}
#second-square {
  background-image: linear-gradient(rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.3)),
    url(../assets/img/news-2.jpg);
  height: 100%;
  background-repeat: no-repeat;
  background-size: cover;
  border-radius: 15px;
}
#third-square {
  background-image: linear-gradient(rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.3)),
    url(../assets/img/news-3.jpg);
  height: 100%;
  background-repeat: no-repeat;
  background-size: cover;
  border-radius: 15px;
}
</style>