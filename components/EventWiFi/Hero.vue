<template>
  <section class="event-wifi-top">
    <div class="container">
      <div class="event-wifi-top-wrapper">
        <h1 class="text-white">Event WiFi</h1>
        <p class="text-white event-wifi-top-text">Tailored WiFi solutions for events and conferences, providing reliable, high-performance connectivity with optional on-site management.</p>
        <div class="text-left">
          <a class="button blue-btn button-icon text-left" href="/contact-us"><span class="btn-effect"> Contact Us</span></a>
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
.event-wifi-top {
  background-image: url("../../assets/images/services/event-wifi-hero.png");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  height: 490px;
}
.event-wifi-top-text {
  font-size: 21px;
}
.event-wifi-top-wrapper {
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: start;
  gap: 31px;
  height: 100%;
}
</style>
