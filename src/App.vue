<template>
  <main>
    <div data-scroll class="container">
      <header class="d-flex align-items-center my-4">
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
        <div class="hero-inner">
          <h1 class="hero-content fade-up">
            <span class="fade-up">With</span>
            <span class="fade-up">you</span>
            <span class="fade-up">every</span>
            <span class="fade-up">step</span>
          </h1>
        </div>
      </div>

      <div class="intro mb-5 fade-up">
        <div class="row">
          <div class="col-sm-6 fade-up" style="animation-delay: 300ms">
            <p>Hosting a conference is a long journey, through complex and sometimes difficult terrain. But the right meeting partner can lighten your load, minimise stress and help you sidestep the pitfalls.</p>
          </div>
          <div class="col-sm-6 fade-up" style="animation-delay: 400ms">
            <p>We are a team you can trust to have your back, to guide, support, advise and problem-solve - and share a laugh along the way.</p>
            <p>
              From the first exploratory steps to the exhilarating finale,
              <strong>we'll be with you every step of the way</strong>.
            </p>
          </div>
        </div>
      </div>

      <div class="line mx-auto my-5"></div>

      <div class="services">
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
      </div>

      <div
        class="numbers p-4 d-flex justify-content-around mb-5"
        data-aos="fade-in"
        v-view.once="runNumbers"
      >
        <div style="flex-basis:220px">
          <h3 class="h5">New Zealand’s leading conference company since 1990</h3>
        </div>
        <div style="flex-basis:100px">
          <div class="label">Awards</div>
          <div class="number">
            <span id="awards">0</span>
            <span>+</span>
          </div>
        </div>
        <div style="flex-basis:100px">
          <div class="label">Employees</div>
          <div class="number">
            <span id="employees">0</span>
            <span>+</span>
          </div>
        </div>
        <div style="flex-basis:120px">
          <div class="label">Successful Projects</div>
          <div class="number">
            <span id="projects">0</span>
            <span>+</span>
          </div>
        </div>
      </div>

      <div class="sections">
        <section class="section row mb-5">
          <div class="section-image-wrapper col-6">
            <div class="section-image">
              <img
                class="img-fluid"
                src="https://res.cloudinary.com/webscope/image/upload/v1568672420/The%20Conference%20Company/img2.png"
              />
            </div>
          </div>
          <div class="section-content col-6 d-flex flex-column justify-content-center">
            <h2 data-aos="fade-up">Who we are</h2>
            <p
              data-aos="fade-up"
              data-aos-delay="200"
            >Our long-serving team offer an extraordinary depth of talent and experience, including specialised skillsets that can add huge value to your project.</p>
            <div data-aos="fade-up" data-aos-delay="400">
              <a class="btn btn-link pl-0" href="#">Meet our team</a>
            </div>
          </div>
        </section>

        <section class="section row mb-5">
          <div class="section-image-wrapper col-6">
            <div class="section-image">
              <img
                class="img-fluid"
                src="https://res.cloudinary.com/webscope/image/upload/v1568843754/The%20Conference%20Company/iapco.png"
              />
            </div>
          </div>
          <div class="section-content col-6 d-flex flex-column justify-content-center">
            <h2 data-aos="fade-up">International Accreditation</h2>
            <p
              data-aos="fade-up"
              data-aos-delay="200"
            >Every year we meet the rigorous accreditation standards of the International Association of Professional Congress Organisers.</p>
            <div data-aos="fade-up" data-aos-delay="400">
              <a class="btn btn-link pl-0" href="#">Learn more</a>
            </div>
          </div>
        </section>
      </div>
    </div>
  </main>
</template>

<script>
import AOS from "aos";
import { CountUp } from "countup.js";
import imagesLoaded from "imagesloaded";

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

    // helper functions
    const MathUtils = {
      // map number x from range [a, b] to [c, d]
      map: (x, a, b, c, d) => ((x - a) * (d - c)) / (b - a) + c,
      // linear interpolation
      lerp: (a, b, n) => (1 - n) * a + n * b,
      // Random float
      getRandomFloat: (min, max) =>
        (Math.random() * (max - min) + min).toFixed(2)
    };

    // body element
    const body = document.body;

    // calculate the viewport size
    let winsize;
    const calcWinsize = () =>
      (winsize = { width: window.innerWidth, height: window.innerHeight });
    calcWinsize();
    // and recalculate on resize
    window.addEventListener("resize", calcWinsize);

    // scroll position
    let docScroll;
    // for scroll speed calculation
    let lastScroll;
    let scrollingSpeed = 0;
    // scroll position update function
    const getPageYScroll = () =>
      (docScroll = window.pageYOffset || document.documentElement.scrollTop);
    window.addEventListener("scroll", getPageYScroll);

    // Item
    class Item {
      constructor(el) {
        // the .item element
        this.DOM = { el: el };
        // the inner image
        this.DOM.image = this.DOM.el.querySelector(".section-image");
        this.DOM.imageWrapper = this.DOM.image.parentNode;

        this.renderedStyles = {
          // here we define which property will change as we scroll the page and the item is inside the viewport
          // in this case we will be:
          // - scaling the inner image
          // - translating the item's title
          // we interpolate between the previous and current value to achieve a smooth effect
          imageScale: {
            // interpolated value
            previous: 0,
            // current value
            current: 0,
            // amount to interpolate
            ease: 0.1,
            // current value setter
            setValue: () => {
              const toValue = 1.3;
              const fromValue = 1;
              const val = MathUtils.map(
                this.props.top - docScroll,
                winsize.height,
                -1 * this.props.height,
                fromValue,
                toValue
              );
              return Math.max(Math.min(val, toValue), fromValue);
            }
          }
        };
        // gets the item's height and top (relative to the document)
        this.getSize();
        // set the initial values
        this.update();
        // use the IntersectionObserver API to check when the element is inside the viewport
        // only then the element styles will be updated
        this.observer = new IntersectionObserver(entries => {
          entries.forEach(
            entry => (this.isVisible = entry.intersectionRatio > 0)
          );
        });
        this.observer.observe(this.DOM.el);
        // init/bind events
        this.initEvents();
      }
      update() {
        // sets the initial value (no interpolation)
        for (const key in this.renderedStyles) {
          this.renderedStyles[key].current = this.renderedStyles[
            key
          ].previous = this.renderedStyles[key].setValue();
        }
        // apply changes/styles
        this.layout();
      }
      getSize() {
        const rect = this.DOM.el.getBoundingClientRect();
        this.props = {
          // item's height
          height: rect.height,
          // offset top relative to the document
          top: docScroll + rect.top
        };
      }
      initEvents() {
        window.addEventListener("resize", () => this.resize());
      }
      resize() {
        // gets the item's height and top (relative to the document)
        this.getSize();
        // on resize reset sizes and update styles
        this.update();
      }
      render() {
        // update the current and interpolated values
        for (const key in this.renderedStyles) {
          this.renderedStyles[key].current = this.renderedStyles[
            key
          ].setValue();
          this.renderedStyles[key].previous = MathUtils.lerp(
            this.renderedStyles[key].previous,
            this.renderedStyles[key].current,
            this.renderedStyles[key].ease
          );
        }

        // and apply changes
        this.layout();
      }
      layout() {
        // scale the image
        this.DOM.image.style.transform = `scale3d(${this.renderedStyles.imageScale.previous},${this.renderedStyles.imageScale.previous},1)`;
      }
    }

    // SmoothScroll
    class SmoothScroll {
      constructor() {
        // the <main> element
        this.DOM = { main: document.querySelector("main") };
        // the scrollable element
        // we translate this element when scrolling (y-axis)
        this.DOM.scrollable = this.DOM.main.querySelector("div[data-scroll]");
        // the items on the page
        this.items = [];
        this.DOM.content = this.DOM.main.querySelector(".sections");
        [...this.DOM.content.querySelectorAll(".section")].forEach(item =>
          this.items.push(new Item(item))
        );
        console.log(this.DOM.content);
        // here we define which property will change as we scroll the page
        // in this case we will be translating on the y-axis
        // we interpolate between the previous and current value to achieve the smooth scrolling effect
        this.renderedStyles = {
          translationY: {
            // interpolated value
            previous: 0,
            // current value
            current: 0,
            // amount to interpolate
            ease: 0.1,
            // current value setter
            // in this case the value of the translation will be the same like the document scroll
            setValue: () => docScroll
          }
        };
        // set the body's height
        this.setSize();
        // set the initial values
        this.update();
        // the <main> element's style needs to be modified
        this.style();
        // init/bind events
        this.initEvents();
        // start the render loop
        requestAnimationFrame(() => this.render());
      }
      update() {
        // sets the initial value (no interpolation) - translate the scroll value
        for (const key in this.renderedStyles) {
          this.renderedStyles[key].current = this.renderedStyles[
            key
          ].previous = this.renderedStyles[key].setValue();
        }
        // translate the scrollable element
        this.layout();
      }
      layout() {
        this.DOM.scrollable.style.transform = `translate3d(0,${-1 *
          this.renderedStyles.translationY.previous}px,0)`;
      }
      setSize() {
        // set the heigh of the body in order to keep the scrollbar on the page
        body.style.height = `${this.DOM.scrollable.scrollHeight}px`;
      }
      style() {
        // the <main> needs to "stick" to the screen and not scroll
        // for that we set it to position fixed and overflow hidden
        this.DOM.main.style.position = "fixed";
        this.DOM.main.style.width = this.DOM.main.style.height = "100%";
        this.DOM.main.style.top = this.DOM.main.style.left = 0;
        this.DOM.main.style.overflow = "hidden";
      }
      initEvents() {
        // on resize reset the body's height
        window.addEventListener("resize", () => this.setSize());
      }
      render() {
        // Get scrolling speed
        // Update lastScroll
        scrollingSpeed = Math.abs(docScroll - lastScroll);
        lastScroll = docScroll;

        // update the current and interpolated values
        for (const key in this.renderedStyles) {
          this.renderedStyles[key].current = this.renderedStyles[
            key
          ].setValue();
          this.renderedStyles[key].previous = MathUtils.lerp(
            this.renderedStyles[key].previous,
            this.renderedStyles[key].current,
            this.renderedStyles[key].ease
          );
        }
        // and translate the scrollable element
        this.layout();

        // for every item
        for (const item of this.items) {
          // if the item is inside the viewport call it's render function
          // this will update item's styles, based on the document scroll value and the item's position on the viewport
          if (item.isVisible) {
            if (item.insideViewport) {
              item.render();
            } else {
              item.insideViewport = true;
              item.update();
            }
          } else {
            item.insideViewport = false;
          }
        }

        // loop..
        requestAnimationFrame(() => this.render());
      }
    }

    /***********************************/
    /********** Preload stuff **********/

    // Preload images
    const preloadImages = () => {
      return new Promise((resolve, reject) => {
        imagesLoaded(
          document.querySelectorAll(".section-image"),
          { background: true },
          resolve
        );
      });
    };

    // And then..
    preloadImages().then(() => {
      // Remove the loader
      document.body.classList.remove("loading");
      // Get the scroll position and update the lastScroll variable
      getPageYScroll();
      lastScroll = docScroll;
      // Initialize the Smooth Scrolling
      new SmoothScroll();
    });
  }
};
</script>

<style lang="scss">
@import "assets/scss/style.scss";

$yellow: #fce300;

.btn {
  border-radius: 0;
}

.line {
  height: 2px;
  width: 50px;
  background-color: $yellow;
}

.label {
  color: #888;
  font-size: 11px;
}

.nav-link {
  color: #000;
}

.btn-link {
  color: #000;
  padding: 10px 0;
  font-weight: bold;
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
  min-height: 650px;
  background-image: url(https://res.cloudinary.com/webscope/image/upload/v1568832314/The%20Conference%20Company/hero.png);
  background-size: cover;
  position: relative;
}

.hero-inner {
  max-width: 900px;
  margin-left: auto;
  margin-right: auto;
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
  width: 260px;
  padding: 30px 30px 0 30px;
  margin-left: -30px;
  margin-bottom: 0;
  font-size: 50px;
  font-weight: bold;
  text-transform: uppercase;
  line-height: 1;
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

.intro {
  max-width: 900px;
  margin-left: auto;
  margin-right: auto;
}

.section {
  &:nth-child(even) {
    .section-image-wrapper {
      order: 2;
    }

    .section-content {
      order: 1;
      padding-left: 100px;
      padding-right: 100px;
    }
  }
  &:nth-child(odd) {
    .section-content {
      padding-left: 100px;
      padding-right: 100px;
    }
  }
}

.section-image-wrapper {
  overflow: hidden;
}

.numbers {
  background: #f6f6f6;
  .number {
    font-size: 50px;
    font-weight: bold;
    line-height: 1;
  }
}

.services {
  display: flex;
  flex-wrap: wrap;
  padding-top: 150px;
  margin-right: -20px;
  margin-left: -20px;
}

.service {
  width: calc(50%);
  padding-left: 20px;
  padding-right: 20px;
  height: 700px;
  margin-bottom: 40px;
  &:nth-child(odd) {
    margin-top: -120px;
  }
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
</style>

