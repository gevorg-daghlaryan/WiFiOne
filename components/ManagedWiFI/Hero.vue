<template>
  <section class="managed-wifi-top">
    <div class="container">
      <div class="managed-wifi-top-wrapper">
        <h1 class="text-white"> Managed WiFi</h1>
        <p class="text-white managed-wifi-top-text">FLorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
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
  background-image: url("../../assets/images/services/wifi.png");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.managed-wifi-top-text {
  font-size: 21px;
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
