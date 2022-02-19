<template>
  <div class="container pt-4">
    <span class="over-the-title">OUR EDITORIAL CONTENT</span>
    <h2>Latest <span class="bck-prim">News</span></h2>
    <div class="row d-flex align-items-center">
      <div class="col-10">
        <p>
          Every week we publish content about what is best in the business
          world.
        </p>
      </div>
      <div class="col-2">
        <button type="button" class="btn btn-outline">SEE ALL</button>
      </div>
    </div>

    <!-- Carte che mostrano persone con scritte -->
    <div class="d-flex justify-content-between pt-4 pb-5">
      <div class="squared text-center">
        <div id="first-square" class="d-flex align-items-end">
          <p>Increasing creativity is possible for everyone</p>
        </div>
      </div>
      <div class="squared text-center">
        <div id="second-square" class="d-flex align-items-end">
          <p>Because market research is parto of the business plan</p>
        </div>
      </div>
      <div class="squared text-center">
        <div id="third-square" class="d-flex align-items-end">
          <p>Working from home is now a trend</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "LatestNews",
  components: {},
  data() {
    return {
      elements: [
        {
          increase: {
            title: "Increasing creativity is possible for everyone",
            img: "../assets/img/news-1.jpg",
            alt: "Studing woman,",
          },

          market: {
            title: "Because market research is parto of the business plan",
            img: "../assets/img/news-2.jpg",
            alt: "Man with sunglasses",
          },
          work: {
            title: "Working from home is now a trend",
            img: "../assets/img/news-3.jpg",
            alt: "Woman with phone and PC",
          },
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";
.squared {
  height: 200px;
  width: 200px;
  p {
    color: white;
    font-size: 0.9rem;
    font-weight: 500;
  }
  #first-square {
    background-image: url("../assets/img/news-1.jpg");
    height: 100%;
    width: 200px;
    background-repeat: no-repeat;
    background-size: cover;
    border-radius: 15px;
  }
  #second-square {
    background-image: url("../assets/img/news-2.jpg");
    height: 100%;
    width: 200px;
    background-repeat: no-repeat;
    background-size: cover;
    border-radius: 15px;
  }
  #third-square {
    background-image: url("../assets/img/news-3.jpg");
    height: 100%;
    width: 200px;
    background-repeat: no-repeat;
    background-size: cover;
    border-radius: 15px;
  }
}

.bck-prim {
  color: $prim_color;
  height: 20px;
  width: 30px;
  background-color: $water_green;
  border-radius: 3px;
}

button {
  background-color: $prim_color;
  color: white;
}

.over-the-title {
  color: $water_green;
  font-size: 0.6rem;
  font-weight: 700;
}

p {
  font-size: 0.6rem;
  color: $text_primary;
}
</style>