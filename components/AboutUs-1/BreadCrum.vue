<template>
  <section class="about-us-top">
      <div class="container">
        <div class="about-us-top-wrapper">
          <h1 class="text-white about-us-top-title">About Us</h1>
          <p class="text-white about-us-top-text">Beyond Connectivity: Get to Know WifiOne – Your Trusted Partner in Transformative Network Solutions.</p>
          <div class="text-left">
            <a class="button blue-btn button-icon text-left" href="/contact-us"><span class="btn-effect"> Contact US</span></a>
          </div>
        </div>
    </div>
  </section>

</template>
<script>
export default {
  name:'BreadCrump'
}
</script>
<style>
  .about-us-top {
    background-image: url("../../assets/images/about-us/hero.png");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    height: 490px;
  }
  .about-us-top-text {
    font-size: 21px;
  }
  .about-us-top-wrapper {
    display: flex;
    flex-direction: column;
    align-items: start;
    justify-content: start;
    gap: 31px;
    height: 100%;
  }
</style>
