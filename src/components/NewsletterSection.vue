<template>
  <div class="h-100" id="know-first">
    <div class="container h-100">
      <div class="row h-100 d-flex align-items-center">
        <div class="col-5 offset-1">
          <span class="over-the-title">NEWSLETTER</span>
          <h2 class="pt-2 pb-2"><span class="bck-prim">Know</span> First</h2>
          <p>
            Follow closely and receive content about our company and the news ot
            the current market.
          </p>
        </div>
        <div class="col-5">
          <form>
            <div class="pb-3">
              <input
                type="text"
                class="form-control form-control-sm"
                placeholder="Name"
              />
            </div>
            <div class="pb-3">
              <input
                type="email"
                class="form-control form-control-sm"
                placeholder="Email"
              />
            </div>

            <button type="submit" class="btn">SUBSCRIBE</button>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "NewsletterSection",
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";

h2 {
  color: white;
}

#know-first {
  background-image: url("../assets/img/bg-1.jpg");
  background-size: cover;
  height: 100%;
  background-repeat: no-repeat;
  background-position: center;
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