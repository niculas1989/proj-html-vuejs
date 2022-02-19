<template>
  <div class="container mt-5">
    <div class="row">
      <div class="col-6">
        <span class="over-the-title">SEND A MESSAGE</span>
        <h2>Get in <span class="bck-prim">Touch</span></h2>
        <p>We will respond to your message as soon as possible.</p>
        <form>
          <div class="row">
            <div class="col-12 pb-3">
              <div class="d-flex">
                <span class="pe-3">
                  <input type="text" placeholder="Name" />
                </span>
                <input type="mail" placeholder="Mail" />
              </div>
            </div>
            <div class="col-12">
              <div class="d-flex">
                <span class="pe-3">
                  <input type="text" placeholder="Phone" />
                </span>
                <input type="text" placeholder="More info" />
              </div>
            </div>
            <div class="col-12 pt-3 w-100">
              <div class="mb-3 w-100">
                <textarea
                  class="form-control w-100"
                  rows="4"
                  placeholder="Message"
                ></textarea>
              </div>
              <button class="btn">SEND</button>
            </div>
          </div>
        </form>
      </div>
      <div class="col-3 offset-1">
        <span><strong>Example Inc.</strong></span>
        <p class="pt-3">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit.
        </p>
        <p>Praesent diam lacus, dapibus sed imperdiet consectur.</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MailSection",
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";

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