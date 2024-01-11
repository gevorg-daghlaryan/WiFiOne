<template>
  <section class="site-monitoring-top">
    <div class="container">
      <div class="site-monitoring-top-wrapper">
        <h1 class="text-white"> Managed WiFi</h1>
        <p class="text-white site-monitoring-top-text">FLorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
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
.site-monitoring-top {
  background-image: url("../../assets/images/services/site-pwer-monitoring-hero.png");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  height: 490px;
}
.site-monitoring-top-text {
  font-size: 21px;
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
