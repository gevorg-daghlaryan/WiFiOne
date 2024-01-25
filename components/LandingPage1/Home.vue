<template>
  <div>
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="7000"
      controls
      fade
      img-width="1024"
      img-height="480"
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <b-carousel-slide
        img-src="../../assets/images/home/slides/slide-1.png"
      >
        <div class="slider-wrapper">
          <div class="slider-content">
            <h2 class="text-white text-left slider-title ">Your Premier WiFi Partner: <br class="d-none d-lg-block">Tailored solutions <br class="d-none d-lg-block">supporting your business</h2>
            <p class="text-white text-left ">Designed-in Quality, Security, and Performance at Zero Upfront Cost</p>
            <div class="text-left">
              <a class="button blue-btn button-icon text-left" href="/contact-us"><span class="btn-effect"> Contact Us</span></a>
            </div>
          </div>
        </div>
      </b-carousel-slide>
      <b-carousel-slide
        img-src="../../assets/images/home/slides/slide-3.png"
      >
        <div class="slider-wrapper">
          <div class="slider-content">
            <h2 class="text-white text-left slider-title ">Event WiFi</h2>
            <p class="text-white text-left ">Enterprice Access Point, LTE or existing <br class="d-none d-lg-block"> backhaul, cloud AP controllers </p>
            <div class="text-left">
              <a class="button blue-btn button-icon text-left" href="/contact-us"><span class="btn-effect"> Contact Us</span></a>
            </div>
          </div>
        </div>
      </b-carousel-slide>
      <b-carousel-slide
        img-src="../../assets/images/home/slides/slide-4.png"
      >
        <div class="slider-wrapper">
          <div class="slider-content">
            <h2 class="text-white text-left slider-title ">Service Industry WiFi </h2>
            <p class="text-white text-left ">Enterprise Access Points and routers, click through portal, <br class="d-none d-lg-block"> Quality of Service, customer and back-office/PoS WiFi</p>
            <div class="text-left">
              <a class="button blue-btn button-icon text-left" href="/contact-us"><span class="btn-effect"> Contact Us</span></a>
            </div>
          </div>
        </div>
      </b-carousel-slide>
      <b-carousel-slide
        img-src="../../assets/images/home/slides/slide-2.png"
      >
        <div class="slider-wrapper">
          <div class="slider-content">
            <h2 class="text-white text-left slider-title ">Integrated Hotel WiFi</h2>
            <p class="text-white text-left ">Customer portal, integration, enterprise Access Points</p>
            <div class="text-left">
              <a class="button blue-btn button-icon text-left" href="/contact-us"><span class="btn-effect"> Contact Us</span></a>
            </div>
          </div>
        </div>
      </b-carousel-slide>
    </b-carousel>
  </div>
</template>

<script>
export default {
  data() {
    return {
      slide: 0,
      sliding: null
    }
  },
  methods: {
    onSlideStart(slide) {
      this.sliding = true
    },
    onSlideEnd(slide) {
      this.sliding = false
    }
  }
}
</script>
<style>
  .slider-content {
    display: flex;
    flex-direction: column;
    justify-content: start;
    gap: 35px;
  }
  .slider-title {
    font-size: 50px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
  }
  .slider-wrapper {
    display: flex;
    flex-direction: row;
    justify-content: start;
    align-items: center;
    width: 100%;
    height: 100%;
  }
  .carousel-caption {
    height: 100%;
  }
  .carousel-item img {
    height: 490px;
    object-fit: cover;
  }
  @media only screen and (max-width: 960px) {
      .slider-title {
        font-size: 20px;
      }
    .slider-content {
      gap: 0;
    }
    }
</style>
