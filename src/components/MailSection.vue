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
              <div id="send-button">
                <button class="btn">SEND</button>
              </div>
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

        <!-- contatti dell'azienda -->
        <div id="contacts">
          <div class="pb-4">
            <i class="fa-solid fa-phone"></i>
            <span> +1(305) 1234-5678</span>
          </div>
          <div class="pb-4">
            <i class="fa-solid fa-envelope"></i>
            <span> hello@example.com</span>
          </div>
          <div class="pb-4">
            <i class="fa-solid fa-location-dot"></i>
            <span> Main Avenue, 987</span>
          </div>
          <div id="button">
            <button class="btn btn-outline-primary">VIEW MAP</button>
          </div>
        </div>
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
#send-button {
  button {
    background-color: $prim_color;
    color: white;
  }
}

#button {
  button {
    border-color: $prim_color;
    color: $prim_color;
    &:hover {
      background-color: $prim_color;
      color: white;
    }
  }
}

#contacts {
  .pb-4 {
    span {
      font-size: 0.8rem;
      color: $prim_color;
    }
    i {
      color: $prim_color;
    }
  }
}

.bck-prim {
  color: $prim_color;
  height: 20px;
  width: 30px;
  background-color: #daeced;
  border-radius: 3px;
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