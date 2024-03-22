<template>
  <div class="carousel-wrapper">
    <ImageLoader v-if="loading" />
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
        id="slide1"
        img-src="/images/home/slides/slide-1.avif"

      >
        <div class="slider-wrapper">
          <div class="slider-content">
            <h2 class="text-white text-left slider-title ">Office-based Businesses</h2>
            <p class="text-white text-left slider-text">Enhance productivity and communication within corporate environments</p>
            <div class="text-left">
              <a class="button blue-btn button-icon text-left" href="/contact-us"><span class="btn-effect"> Contact Us</span></a>
            </div>
          </div>
        </div>
      </b-carousel-slide>
      <b-carousel-slide
        img-src="/images/home/slides/slide-2.avif"
      >
        <div class="slider-wrapper">
          <div class="slider-content">
            <h2 class="text-white text-left slider-title ">Event Management Companies</h2>
            <p class="text-white text-left slider-text">Providing reliable WiFi solutions during events and conferences</p>
            <div class="text-left">
              <a class="button blue-btn button-icon text-left" href="/contact-us"><span class="btn-effect"> Contact Us</span></a>
            </div>
          </div>
        </div>
      </b-carousel-slide>
      <b-carousel-slide
        img-src="/images/home/slides/slide-3.avif"
      >
        <div class="slider-wrapper">
          <div class="slider-content">
            <h2 class="text-white text-left slider-title ">Hotels and Hospitality Businesses</h2>
            <p class="text-white text-left slider-text">Elevate your guest experience with seamless and secure connectivity</p>
            <div class="text-left">
              <a class="button blue-btn button-icon text-left" href="/contact-us"><span class="btn-effect"> Contact Us</span></a>
            </div>
          </div>
        </div>
      </b-carousel-slide>
      <b-carousel-slide
        img-src="/images/home/slides/slide-4.avif"
      >
        <div class="slider-wrapper">
          <div class="slider-content">
            <h2 class="text-white text-left slider-title ">Event WiFi</h2>
            <p class="text-white text-left slider-text">Tailored WiFi solutions for events and conferences, providing reliable,  high-performance connectivity with optional on-site management</p>
            <div class="text-left">
              <a class="button blue-btn button-icon text-left" href="/contact-us"><span class="btn-effect"> Contact Us</span></a>
            </div>
          </div>
        </div>
      </b-carousel-slide>
      <b-carousel-slide
        img-src="/images/home/slides/slide-5.avif"
      >
        <div class="slider-wrapper">
          <div class="slider-content">
            <h2 class="text-white text-left slider-title ">Managed Cameras</h2>
            <p class="text-white text-left slider-text">Oversight and management of security cameras and access systems, enhancing safety and surveillance for businesses</p>
            <div class="text-left">
              <a class="button blue-btn button-icon text-left" href="/contact-us"><span class="btn-effect"> Contact Us</span></a>
            </div>
          </div>
        </div>
      </b-carousel-slide>
      <b-carousel-slide
        img-src="/images/home/slides/slide-6.avif"
      >
        <div class="slider-wrapper">
          <div class="slider-content">
            <h2 class="text-white text-left slider-title ">Managed Music Systems</h2>
            <p class="text-white text-left slider-text">Centralized control and management of multi-zone speaker systems for optimized audio experiences in various areas</p>
            <div class="text-left">
              <a class="button blue-btn button-icon text-left" href="/contact-us"><span class="btn-effect"> Contact Us</span></a>
            </div>
          </div>
        </div>
      </b-carousel-slide>
      <b-carousel-slide
        img-src="/images/home/slides/slide-7.avif"
      >
        <div class="slider-wrapper">
          <div class="slider-content">
            <h2 class="text-white text-left slider-title ">Site Power Monitoring</h2>
            <p class="text-white text-left slider-text">Giving you immediate notification when power fails on one of your sites</p>
            <div class="text-left">
              <a class="button blue-btn button-icon text-left" href="/contact-us"><span class="btn-effect"> Contact Us</span></a>
            </div>
          </div>
        </div>
      </b-carousel-slide>
      <b-carousel-slide
        img-src="/images/home/slides/slide-8.avif"
      >
        <div class="slider-wrapper">
          <div class="slider-content">
            <h2 class="text-white text-left slider-title ">Managed Media Wall</h2>
            <p class="text-white text-left slider-text">Get your message out with vivid and fluid graphics and video</p>
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
import ImageLoader from "~/components/themes/ImageLoader.vue";

export default {
  components: {ImageLoader},
  data() {
    return {
      slide: 0,
      sliding: null,
      loading: true,
    }
  },
  methods: {
    onSlideStart(slide) {
      this.sliding = true
    },
    onSlideEnd(slide) {
      this.sliding = false
    }
  },
  mounted() {
    const backgroundImage = new Image();
    backgroundImage.src = "/images/home/slides/slide-1.webp";
    backgroundImage.onload = () => {
      this.loading = false;
    };
    backgroundImage.onerror = () => {
      this.loading = false;
    };
  },
}
</script>
<style>
  .carousel-wrapper {
    position: relative;
    min-height: 490px;
    background-color: #dedede;
    //opacity: 0.5;
  }
  .slider-content {
    display: flex;
    flex-direction: column;
    justify-content: start;
    gap: 20px;
  }
  .slider-title {
    font-size: 50px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
  }
  .slider-text {
    font-size: 21px;
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
