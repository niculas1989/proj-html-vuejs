<template>
  <div id="footer-page" class="d-flex flex-column justify-content-between">
    <div class="container pt-5">
      <div class="row">
        <div class="col-3">
          <div class="text-center">
            <h5><span class="bck-prim">NEXT</span> GEN</h5>
            <p>A Functional HTML Template for Corporate & Business.</p>
            <div class="pb-1">
              <i class="fa-solid fa-phone"></i>
              <p class="d-inline ps-2">+1(305) 1234-5678</p>
            </div>
            <div class="pb-1">
              <i class="fa-solid fa-envelope"></i>
              <p class="d-inline ps-2">hello@example.com</p>
            </div>
            <div class="pb-3">
              <i class="fa-solid fa-location-dot"></i>
              <p class="d-inline ps-2">Main Avenue, 987</p>
            </div>
            <div id="button">
              <button class="btn btn-outline-primary">GET IN TOUCH</button>
            </div>
          </div>
        </div>

        <div class="col-3">
          <div class="square">
            <ul>
              <li>
                <h6 class="pt-3">About</h6>
              </li>
              <li class="pt-2">
                <a href="#"> > The Company </a>
              </li>
              <li>
                <a href="#">> Insitutional</a>
              </li>
              <li>
                <a href="#">> Social & Events</a>
              </li>
              <li>
                <a href="#">> Innovation</a>
              </li>
              <li>
                <a href="#">> Environment</a>
              </li>
              <li>
                <a href="#">> Technology</a>
              </li>
            </ul>
          </div>
        </div>
        <div class="col-3">
          <div class="square">
            <ul>
              <li>
                <h6 class="pt-3">Services</h6>
              </li>
              <li class="pt-2">
                <a href="#"> > Audit & Assurance </a>
              </li>
              <li>
                <a href="#">> Financial Advisory</a>
              </li>
              <li>
                <a href="#">> Analystic Advisory</a>
              </li>
              <li>
                <a href="#">> Middle Marketing</a>
              </li>
              <li>
                <a href="#">> Legal consulting</a>
              </li>
              <li>
                <a href="#">> Regulatory Risk</a>
              </li>
            </ul>
          </div>
        </div>
        <div class="col-3">
          <div class="square">
            <ul>
              <li>
                <h6 class="pt-3">Support</h6>
              </li>
              <li class="pt-2">
                <a href="#"> > Responsability </a>
              </li>
              <li>
                <a href="#">> Term of Use</a>
              </li>
              <li>
                <a href="#">> About Cookies</a>
              </li>
              <li>
                <a href="#">> Privacy Policy</a>
              </li>
              <li>
                <a href="#">> Accessibility</a>
              </li>
              <li>
                <a href="#">> Information</a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div id="bottom-footer" class="position-relative">
      <a href="up">
        <div class="arrow-up">
          <i class="fa-solid fa-arrow-up"></i>
        </div>
      </a>
      <div class="container h-100">
        <div class="d-flex justify-content-between align-items-center h-100">
          <span
            >Enjoy the low price. We are tracking any intention of piracy</span
          >
          <span>
            <i class="fa-regular fa-copyright"></i>
            2022 NEXGEN is Proudly Powered by
            <span id="proud">Boolean</span> Student with
            <i class="fa-solid fa-heart"></i>
          </span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterPage",
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";

.arrow-up {
  position: absolute;
  right: 15px;
  top: 12px;
  height: 30px;
  width: 30px;
  background-color: #19191c;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
}
a {
  color: #000;
  &:hover {
    transform: translateY(-10px);
    color: $prim_color;
  }
}

#footer-page {
  height: 350px;
  background-color: $background_dark;
  #bottom-footer {
    height: 50px;
    background-color: #000;
    span {
      font-size: 0.6rem;
      color: $text_primary;
    }
    .fa-heart {
      color: darkred;
    }
    #proud {
      color: $prim_color;
    }
  }
}

ul,
li {
  list-style-type: none;
  font-size: 0.6rem;
  color: $text_primary;
  padding-bottom: 0.3rem;
  h6 {
    color: white;
  }
}

.square {
  height: 200px;
  background-color: $background_single_card;
  border-radius: 5px;
  a {
    color: $text_primary;
    text-decoration: none;
    &:hover {
      color: $prim_color;
    }
  }
}

.bck-prim {
  color: $water_green;
  height: 20px;
  width: 30px;
  background-color: #0e272d;
  border-radius: 3px;
}

.container {
  color: white;
  button {
    border-color: $prim_color;
    color: white;
    &:hover {
      background-color: $prim_color;
      color: white;
    }
  }
}

p {
  font-size: 0.6rem;
  color: $text_primary;
}
</style>