<template>
  <section class="managed-wifi-top py-0">
    <video  autoplay loop class="video-background" poster="../../assets/images/services/wifi.webp">
      <source src="/videos/manag-wifi.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <img class="image-foreground" src="../../assets/images/services/wifi.webp" alt="hero">
    <div class="container">
      <div class="managed-wifi-top-wrapper">
        <h1 class="text-whit managed-wifi-top-title"> Managed WiFi</h1>
        <p class="text-white managed-wifi-top-text">Comprehensive management of WiFi and network infrastructure,</p>
        <div class="text-left">
          <a class="button blue-btn button-icon text-left" href="/contact-us"><span class="btn-effect"> Contact US</span></a>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name:'Hero'
}
</script>
<style>
.managed-wifi-top {
  position: relative;
  display: flex;
  align-items: center;
  height: 500px;
}
.managed-wifi-top-text {
  font-size: 21px;
  z-index: 10 !important;

}
.managed-wifi-top-title {
  z-index: 10;
  color: #FFFFFF !important;
}
.managed-wifi-top-wrapper {
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: start;
  gap: 31px;
  height: 100%;
}
.image-foreground {
  position: absolute;
  object-fit: cover;
  height: 100%;
  width: 100%;
  mix-blend-mode: lighten;
  z-index: 2;
}
.video-background{
  position: absolute;
  height: 100%;
  width: 100%;
  object-fit: cover;
  z-index: 1;
}
</style>
