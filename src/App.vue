<template>
  <main>
    <div data-scroll>
      <header class="container d-flex align-items-center my-4">
        <div>
          <img
            src="https://res.cloudinary.com/webscope/image/upload/v1568745889/The%20Conference%20Company/logo.png"
          />
        </div>
        <ul class="nav ml-auto">
          <li class="nav-item">
            <a class="nav-link" href="#">Services +</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Our Work</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">About Us</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Contact</a>
          </li>
        </ul>
      </header>
      <div id="hero" class="hero mb-5 fade-up" style="animation-duration: 1200ms">
        <div class="hero-inner container">
          <h1 class="hero-content fade-up">
            <span class="fade-up">With</span>
            <span class="fade-up">you</span>
            <span class="fade-up">every</span>
            <span class="fade-up">step</span>
          </h1>
        </div>
      </div>

      <div class="sections container">
        <div class="intro mb-5 pb-5 border-bottom fade-up">
          <div class="row mb-4">
            <div class="col-sm-4 fade-up" style="animation-delay: 300ms">
              <p>Hosting a conference is a long journey, through complex and sometimes difficult terrain. But the right meeting partner can lighten your load, minimise stress and help you sidestep the pitfalls.</p>
            </div>
            <div class="col-sm-4 fade-up" style="animation-delay: 400ms">
              <p>We are a team you can trust to have your back, to guide, support, advise and problem-solve - and share a laugh along the way.</p>
            </div>
            <div class="col-sm-4 fade-up" style="animation-delay: 500ms">
              <p>
                From the first exploratory steps to the exhilarating finale,
                <strong>we'll be with you every step of the way</strong>.
              </p>
            </div>
          </div>
          <div class="text-center">
            <button class="btn btn-primary">Talk to an expert</button>
          </div>
        </div>

        <!-- <div class="services">
          <a
            href="#"
            class="service"
            data-aos="fade-up"
            :data-aos-delay="index * 50"
            v-for="(service, index) in services"
            :key="service.name"
          >
            <div class="service-inner" :style="{background: `url(${service.img})`}">
              <div class="overlay"></div>
              <div class="service-content">
                <h3 class="service-name">{{service.name}}</h3>
                <p class="service-blurb mb-4">{{service.blurb}}</p>
                <div class="service-link text-center">
                  <div class="btn btn-outline-light">Learn More</div>
                </div>
              </div>
            </div>
          </a>
        </div>-->

        <div class="services">
          <div class="row">
            <div class="col-sm-8">
              <a href="#" class="service service-lg" data-aos="fade-up" data-aos-delay="50">
                <div
                  class="service-inner"
                  style="background: url(https://res.cloudinary.com/webscope/image/upload/c_fill,f_auto,g_faces,h_480,w_756/v1569188045/The%20Conference%20Company/CoreNet_Symposium_LR-513_-_credited_3.jpg)"
                >
                  <div class="overlay"></div>
                  <div class="service-content">
                    <h3 class="service-name">Conferences & Meetings</h3>
                    <p
                      class="service-blurb mb-4"
                    >We offer a comprehensive meeting management service, available full-menu or à la carte, plus strategic advice and consultancy.</p>
                    <div class="service-link text-center">
                      <div class="btn btn-outline-light">Learn More</div>
                    </div>
                  </div>
                </div>
              </a>
            </div>
            <div class="col-sm-4">
              <a href="#" class="service service-sm" data-aos="fade-up" data-aos-delay="50">
                <div
                  class="service-inner"
                  style="background: url(https://res.cloudinary.com/webscope/image/upload/c_fit,f_auto,h_480,w_364/v1568795552/The%20Conference%20Company/img3.png)"
                >
                  <div class="overlay"></div>
                  <div class="service-content">
                    <h3 class="service-name">International Conference Bids</h3>
                    <p
                      class="service-blurb mb-4"
                    >Considering hosting an international event? We can help craft all elements of your bid, from an accurate bid budget to a compelling sales pitch.</p>
                    <div class="service-link text-center">
                      <div class="btn btn-outline-light">Learn More</div>
                    </div>
                  </div>
                </div>
              </a>
            </div>
          </div>
          <div class="row">
            <div class="col-sm-4">
              <a href="#" class="service service-sm" data-aos="fade-up" data-aos-delay="50">
                <div
                  class="service-inner"
                  style="background: url(https://res.cloudinary.com/webscope/image/upload/c_fit,f_auto,h_480,w_364/v1568795552/The%20Conference%20Company/img5.png)"
                >
                  <div class="overlay"></div>
                  <div class="service-content">
                    <h3 class="service-name">Awards Managment</h3>
                    <p
                      class="service-blurb mb-4"
                    >Our specialist ‘one-stop’ awards company offers an end-to-end awards management service, from coordinating entries and judging to the final celebration.</p>
                    <div class="service-link text-center">
                      <div class="btn btn-outline-light">Learn More</div>
                    </div>
                  </div>
                </div>
              </a>
            </div>
            <div class="col-sm-8">
              <a href="#" class="service service-lg" data-aos="fade-up" data-aos-delay="50">
                <div
                  class="service-inner"
                  style="background: url(https://res.cloudinary.com/webscope/image/upload/c_scale,h_480,w_756/v1569189055/The%20Conference%20Company/WSAVA_Thur-1161_0.jpg)"
                >
                  <div class="overlay"></div>
                  <div class="service-content">
                    <h3 class="service-name">Corporate Events</h3>
                    <p
                      class="service-blurb mb-4"
                    >We’ll make sure every aspect of your event is designed to give your messages maximum impact, from concept to delivery.</p>
                    <div class="service-link text-center">
                      <div class="btn btn-outline-light">Learn More</div>
                    </div>
                  </div>
                </div>
              </a>
            </div>
          </div>
        </div>

        <section class="section row mb-5">
          <div class="col-sm-4">
            <div class="border-top border-bottom h-100 py-5">
              <h2 data-aos="fade-up" class="h5 font-weight-semibold">Who we are</h2>
            </div>
          </div>

          <div class="section-content col-sm-8">
            <div class="border-top border-bottom py-5">
              <div class="row">
                <div class="col-sm-6">
                  <p
                    data-aos="fade-up"
                    data-aos-delay="200"
                  >Our long-serving team offer an extraordinary depth of talent and experience, including specialised skillsets that can add huge value to your project.</p>
                  <div data-aos="fade-up" data-aos-delay="400">
                    <a class="btn btn-link pl-0" href="#">Meet our team</a>
                  </div>
                </div>
                <div class="col-sm-6">
                  <div class="section-image-wrapper">
                    <div class="section-image">
                      <img
                        class="img-fluid"
                        src="https://res.cloudinary.com/webscope/image/upload/v1568672420/The%20Conference%20Company/img2.png"
                      />
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </section>

        <div
          class="numbers py-4 d-flex justify-content-between mb-5"
          data-aos="fade-in"
          v-view.once="runNumbers"
        >
          <div style="flex-basis:220px">
            <h3
              class="h5 mb-0"
              data-aos="fade-up"
            >New Zealand’s leading conference company since 1990</h3>
          </div>
          <div style="flex-basis:100px" data-aos="fade-up" data-aos-delay="200">
            <div class="label">Awards</div>
            <div class="number">
              <span id="awards">0</span>
              <span>+</span>
            </div>
          </div>
          <div style="flex-basis:100px" data-aos="fade-up" data-aos-delay="400">
            <div class="label">Employees</div>
            <div class="number">
              <span id="employees">0</span>
              <span>+</span>
            </div>
          </div>
          <div style="flex-basis:120px" data-aos="fade-up" data-aos-delay="600">
            <div class="label">Successful Projects</div>
            <div class="number">
              <span id="projects">0</span>
              <span>+</span>
            </div>
          </div>
        </div>

        <section class="section row mb-5">
          <div class="col-sm-4">
            <div class="border-top pt-5">
              <h2 data-aos="fade-up" class="h5">
                International
                <br />Accreditation
              </h2>
            </div>
          </div>

          <div class="section-content col-sm-8">
            <div class="border-top pt-5">
              <div class="row">
                <div class="col-sm-6">
                  <p
                    data-aos="fade-up"
                    data-aos-delay="200"
                  >Every year we meet the rigorous accreditation standards of the International Association of Professional Congress Organisers.</p>
                  <div data-aos="fade-up" data-aos-delay="400">
                    <a class="btn btn-link pl-0" href="#">Learn More</a>
                  </div>
                </div>
                <div class="col-sm-6">
                  <div class="section-image-wrapper">
                    <div class="section-image">
                      <img
                        class="img-fluid"
                        src="https://res.cloudinary.com/webscope/image/upload/v1568843754/The%20Conference%20Company/iapco.png"
                      />
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </section>

        <div class="border-top py-5">
          <h3 class="h5 mb-3" data-aos="fade-up">What's on our minds</h3>
          <div class="row">
            <div class="col-sm-3" data-aos="fade-up" data-aos-delay="200">
              <div class="img-wrapper mb-2 position-relative">
                <img
                  class="img-fluid"
                  src="https://www.theconferencecompany.com/sites/default/files/styles/hero_med_color/public/2018-05/IAPCO%20EDGE%20Taipei%200421_1_0.jpg?itok=5dgFu7ie"
                />
                <span class="label-yellow">Article</span>
              </div>
              <p class="text-sm">What is ‘CQ’, and why is it so vital to the meetings industry?</p>
            </div>
            <div class="col-sm-3" data-aos="fade-up" data-aos-delay="400">
              <div class="img-wrapper mb-2 position-relative">
                <img
                  class="img-fluid"
                  src="https://www.theconferencecompany.com/sites/default/files/styles/hero_med_color/public/2019-07/Ella%201.JPG?h=e5aec6c8&itok=ph05PpoN"
                />
                <span class="label-yellow">Article</span>
              </div>
              <p class="text-sm">Welcome to The Conference Company, Ella!</p>
            </div>
            <div class="col-sm-3" data-aos="fade-up" data-aos-delay="600">
              <div class="img-wrapper mb-2 position-relative">
                <img
                  class="img-fluid"
                  src="https://www.theconferencecompany.com/sites/default/files/styles/hero_large/public/2018-05/00554_1.JPG?itok=K2quBS6w"
                />
                <span class="label-yellow">Project</span>
              </div>
              <p class="text-sm">Australia and New Zealand Endovascular Therapies Annual Meeting</p>
            </div>
            <div class="col-sm-3" data-aos="fade-up" data-aos-delay="800">
              <div class="img-wrapper mb-2 position-relative">
                <img
                  class="img-fluid"
                  src="https://www.theconferencecompany.com/sites/default/files/styles/hero_med_color/public/2018-09/Moderators_0.jpg?itok=teoyo6uy"
                />
                <span class="label-yellow">Project</span>
              </div>
              <p class="text-sm">Leading from the front: why the moderator makes the conference</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>

<script>
import AOS from "aos";
import { CountUp } from "countup.js";
import imagesLoaded from "imagesloaded";
import { smoothScroll } from "./plugins/smoothScroll";

export default {
  name: "App",
  data() {
    return {
      loading: false,
      services: [
        {
          name: "Conferences & Meetings",
          blurb:
            "We offer a comprehensive meeting management service, available full-menu or à la carte, plus strategic advice and consultancy.",
          img:
            "https://res.cloudinary.com/webscope/image/upload/v1568672192/The%20Conference%20Company/img1.png"
        },
        {
          name: "International Conference Bids",
          blurb:
            "Considering hosting an international event? We can help craft all elements of your bid, from an accurate bid budget to a compelling sales pitch.",

          img:
            "https://res.cloudinary.com/webscope/image/upload/v1568795552/The%20Conference%20Company/img3.png"
        },
        {
          name: "Corporate Events",
          blurb:
            "We’ll make sure every aspect of your event is designed to give your messages maximum impact, from concept to delivery.",

          img:
            "https://res.cloudinary.com/webscope/image/upload/v1568795552/The%20Conference%20Company/img4.png"
        },
        {
          name: "Awards Managment",
          blurb:
            "Our specialist ‘one-stop’ awards company offers an end-to-end awards management service, from coordinating entries and judging to the final celebration.",

          img:
            "https://res.cloudinary.com/webscope/image/upload/v1568795552/The%20Conference%20Company/img5.png"
        }
      ]
    };
  },
  methods: {
    runNumbers() {
      setTimeout(function() {
        var awards = new CountUp("awards", 80);
        awards.start();

        var employees = new CountUp("employees", 35);
        employees.start();

        var projects = new CountUp("projects", 250);
        projects.start();
      }, 1000);
    }
  },
  mounted() {
    AOS.init({
      duration: 800,
      easing: "ease-out-quad"
    });
    smoothScroll(imagesLoaded);
  }
};
</script>

<style lang="scss">
@import "assets/scss/style.scss";

$yellow: #fce300;

.btn {
  border-radius: 0;
  font-weight: 500;
  padding: 0.5rem 1rem;
}

.btn-primary {
  background-color: $yellow;
  border: none;
  color: #000;
}

.line {
  height: 2px;
  width: 50px;
  margin-bottom: 5px;
  background-color: $yellow;
}

.label {
  color: #888;
  font-size: 12px;
}

.nav-link {
  color: #000;
}

.btn-link {
  color: #000;
  padding: 10px 0;
  // font-weight: bold;
  position: relative;
  &:hover {
    text-decoration: none;
    color: #666;
  }
  &::before {
    content: "";
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    z-index: -1;
    height: 3px;
    width: 100%;
    background-color: $yellow;
  }
}

.hero {
  max-width: 1400px;
  margin-left: auto;
  margin-right: auto;
  min-height: 650px;
  background-image: url(https://res.cloudinary.com/webscope/image/upload/v1568832314/The%20Conference%20Company/hero.png);
  background-size: cover;
  position: relative;
}

.hero-inner {
  // max-width: 900px;
  // margin-left: auto;
  // margin-right: auto;
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
}

@keyframes fadeUp {
  from {
    opacity: 0;
    transform: translate3D(0, 30px, 0);
  }
  to {
    opacity: 1;
    transform: none;
  }
}

.fade-up {
  opacity: 0;
  animation-name: fadeUp;
  animation-duration: 600ms;
  animation-timing-function: cubic-bezier(0.165, 0.84, 0.44, 1);
  animation-fill-mode: forwards;
}

.hero-content {
  background-color: #fff;
  border-left: 5px solid $yellow;
  width: 260px;
  padding: 30px 30px 0 30px;
  margin-left: -30px;
  margin-bottom: 0;
  font-size: 50px;
  font-weight: bold;
  text-transform: uppercase;
  line-height: 1.1;
  span {
    display: block;

    &:nth-child(2) {
      animation-delay: 150ms;
    }
    &:nth-child(3) {
      animation-delay: 200ms;
    }
    &:nth-child(4) {
      animation-delay: 250ms;
    }
  }
}

// .intro {
//   max-width: 900px;
//   margin-left: auto;
//   margin-right: auto;
// }

// .section {
//   &:nth-child(even) {
//     .section-image-wrapper {
//       order: 2;
//     }

//     .section-content {
//       order: 1;
//       padding-left: 100px;
//       padding-right: 100px;
//     }
//   }
//   &:nth-child(odd) {
//     .section-content {
//       padding-left: 100px;
//       padding-right: 100px;
//     }
//   }
// }

.section-image-wrapper {
  overflow: hidden;
}

.numbers {
  // background: #f6f6f6;
  .number {
    font-size: 50px;
    font-weight: 500;
    line-height: 1;
  }
}

.service {
  display: block;
  height: 480px;
  margin-bottom: 40px;
  &:hover {
    .service-content {
      top: 50%;
    }
    .service-blurb {
      opacity: 1;
      transform: none;
    }
    .service-link {
      opacity: 1;
      transform: none;
    }
    .overlay {
      transform: none;
    }
  }
}

.service-sm {
  &:hover {
    .service-content {
      top: 30%;
    }
  }
}

.service-inner {
  position: relative;
  height: 100%;
  color: #fff;
  padding-left: 80px;
  padding-right: 80px;
  overflow: hidden;
  .overlay {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    height: 100%;
    transform: translateY(50%);
    transition: transform 450ms ease;
    background: linear-gradient(
      0deg,
      rgba(0, 0, 0, 1) 0%,
      rgba(0, 0, 0, 0) 100%
    );
  }
}

.service-content {
  position: absolute;
  top: 80%;
  left: 50%;
  width: 70%;
  transform: translateX(-50%);
  transition: all 450ms ease-in-out;
}

.service-name {
  text-align: center;
  font-size: 24px;
  margin-bottom: 30px;
}

.service-blurb {
  opacity: 0;
  transform: translateY(20px);
  transition: all 450ms ease-in-out 150ms;
}

.service-link {
  opacity: 0;
  transform: translateY(30px);
  transition: all 450ms ease-in-out 200ms;
}

.label-yellow {
  position: absolute;
  bottom: 0;
  left: 0;
  background-color: $yellow;
  display: inline-block;
  font-size: 10px;
  font-weight: 500;
  text-transform: uppercase;
  letter-spacing: 1px;
  color: #000;
  padding: 3px 5px 2px;
  margin-bottom: 10px;
}

.img-wrapper {
  overflow: hidden;
  img {
    transition: transform 300ms ease-in-out;
    transform: translateZ(0) scale(1); // TranslateZ seems to reduce blurriness
  }
  &:hover {
    img {
      transform: scale(1.1);
    }
  }
}
</style>

