<template>
  <section class="site-monitoring-top" id="siteMonitoringTopSection">
    <ImageLoader v-if="loading" />
    <div class="container">
      <div class="site-monitoring-top-wrapper">
        <h1 class="text-white"> Site Power Monitoring</h1>
        <p class="text-white site-monitoring-top-text">Giving you immediate notification when power fails on one of your sites</p>
        <div class="text-left">
          <a class="button blue-btn button-icon text-left" href="/contact-us"><span class="btn-effect"> Contact Us</span></a>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import ImageLoader from "~/components/themes/ImageLoader.vue";

export default {
  name:'Hero',
  components: {ImageLoader},
  data() {
    return {
      loading: true,
    };
  },
  mounted() {
    const section = document.getElementById('siteMonitoringTopSection');
    const backgroundImage = new Image();
    backgroundImage.src = "/images/services/site-pwr-monitoring-hero.avif";
    backgroundImage.onload = () => {
      section.classList.add('site-power-monitoring-top-image-loaded');
      this.loading = false;
    };
    backgroundImage.onerror = () => {
      section.classList.add('site-power-monitoring-top-image-loaded');
      this.loading = false;
    };
  },
}
</script>
<style>
.site-monitoring-top {
  position: relative;
  background-image: url("/images/services/site-pwr-monitoring-hero.avif");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  background-color: #dedede;
  height: 490px;
}
.site-monitoring-top-text {
  font-size: 21px;
}
.site-power-monitoring-top-image-loaded {
  background-image: url("/images/services/site-pwr-monitoring-hero.avif");
}
.site-monitoring-top-wrapper {
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: start;
  gap: 31px;
  height: 100%;
}
</style>
