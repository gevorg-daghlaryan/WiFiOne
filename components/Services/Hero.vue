<template>
  <section class="service-top">
    <div class="container">
      <div class="service-top-wrapper">
        <h1 class="text-white"> Services</h1>
        <p class="text-white service-top-text">From scalable connectivity solutions to proactive security measures, we deliver performance and
          <br> reliability, empowering your business operations</p>
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
.service-top {
  background-image: url("../../assets/images/services/hero.png");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.service-top-text {
  font-size: 21px;
}
.service-top-wrapper {
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: start;
  gap: 31px;
  height: 100%;
}
</style>
