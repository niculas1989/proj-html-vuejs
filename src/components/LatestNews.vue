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
      <GenerateCards :item="elements" />
    </div>
  </div>
</template>

<script>
import GenerateCards from "./GenerateCards.vue";
export default {
  name: "LatestNews",
  components: {
    GenerateCards,
  },
  data() {
    return {
      hover: false,
      elements: [
        {
          title: "Increasing creativity is possible for everyone",
          img: "news-1.jpg",
          alt: "Studing woman,",
        },
        {
          title: "Because market research is parto of the business plan",
          img: "news-2.jpg",
          alt: "Man with sunglasses",
        },
        {
          title: "Working from home is now a trend",
          img: "news-3.jpg",
          alt: "Woman with phone and PC",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";

.bck-prim {
  color: $prim_color;
  height: 20px;
  width: 30px;
  background-color: #daeced;
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