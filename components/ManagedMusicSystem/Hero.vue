<template>
  <section class="managed-music-top" id="managedMusicSystemTopSection">
    <ImageLoader v-if="loading" />
    <div class="container">
      <div class="row flex-nowrap">
        <div class="col-lg-10">
          <div class="managed-music-top-wrapper">
            <div class="wrapper-managed-music-title">
            <h1 class="text-white">Managed Music System</h1>
            </div>
            <p class="text-white managed-music-top-text">Centralized control and management of multi-zone speaker systems for optimized audio
              <br> experiences in various areas.</p>
            <div class="text-left">
              <a class="button blue-btn button-icon text-left" href="/contact-us"><span class="btn-effect"> Contact Us</span></a>
            </div>
          </div>
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
    const section = document.getElementById('managedMusicSystemTopSection');
    const backgroundImage = new Image();
    backgroundImage.src = "/images/services/manag-music-hero.avif";
    backgroundImage.onload = () => {
      section.classList.add('managed-music-system-top-image-loaded');
      this.loading = false;
    };
    backgroundImage.onerror = () => {
      section.classList.add('managed-music-system-top-image-loaded');
      this.loading = false;
    };
  },
}
</script>
<style>
  .managed-music-top {
    position: relative;
    background-image: url("/images/services/manag-music-hero.avif");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    background-color: #dedede;
  }
  .managed-music-top-text {
    font-size: 21px;
  }
  .managed-music-top-wrapper {
    display: flex;
    flex-direction: column;
    align-items: start;
    justify-content: start;
    gap: 31px;
    height: 100%;
  }
  .wrapper-managed-music-title {
    width: 100%;
    display: flex;
    justify-content: space-between;
  }
</style>
