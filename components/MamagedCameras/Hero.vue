<template>
  <section class="managed-cameras-top">
    <div class="container">
      <div class="managed-cameras-top-wrapper">
        <h1 class="text-white"> Managed Cameras</h1>
        <p class="text-white managed-cameras-top-text">FLorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
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
.managed-cameras-top {
  background-image: url("../../assets/images/services/manag-cam-hero.png");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  height: 490px;
}
.managed-cameras-top-text {
  font-size: 21px;
}
.managed-cameras-top-wrapper {
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: start;
  gap: 31px;
  height: 100%;
}
</style>
