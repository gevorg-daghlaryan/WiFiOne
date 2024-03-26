<template>
  <section class="managed-wifi-top" id="managedWiFITopSection">
    <ImageLoader v-if="loading" />
    <div class="container">
      <div class="managed-wifi-top-wrapper">
        <h1 class="text-white">Managed WiFi</h1>
        <p class="text-white managed-media-wall-top-text">Comprehensive management of WiFi and network infrastructure</p>
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
    const section = document.getElementById('managedWiFITopSection');
    const backgroundImage = new Image();
    backgroundImage.src = "/images/services/manag-wifi.avif";
    backgroundImage.onload = () => {
      section.classList.add('managed-media-wall-top-image-loaded');
      this.loading = false;
    };
    backgroundImage.onerror = () => {
      section.classList.add('managed-media-wall-top-image-loaded');
      this.loading = false;
    };
  },
}
</script>
<style>
.managed-wifi-top {
  position: relative;
  background-image: url("/images/services/manag-wifi.avif");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  background-color: #dedede;
  height: 490px;
}
.managed-media-wall-top-text {
  font-size: 21px;
}
.managed-media-wall-top-image-loaded {
  background-image: url("/images/services/manag-wifi.avif");
}
.managed-wifi-top-wrapper {
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: start;
  gap: 31px;
  height: 100%;
}
</style>
