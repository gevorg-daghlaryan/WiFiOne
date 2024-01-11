<template>
  <section class="advantages-section">
    <div class="container">
      <div class="row">
        <div class="col-lg-8 col-sm-12 sidebar-service-left">
          <h1 class="advantages-title mb-3">Unique Advantages</h1>
          <ul class="advantages-list">
            <li>Careful coverage and equipment layout for strong WiFi throughout your site</li>
            <li>Leading US-brand enterprise equipment at a low operating cost</li>
            <li>Secure network design to limit malware and intrusion</li>
            <li>Bespoke Access Point mounting system for stronger signal</li>
          </ul>
        </div>
        <div class="col-lg-4 col-sm-12 pt-5 pt-lg-0">
          <img src="../../assets/images/services/manag-wifi.png" alt="">
        </div>
      </div>
    </div>
  </section>
</template>
<script >
export default {
  name: 'Advantages',
}
</script>

<style>
  .advantages-title {
    color: rgba(52, 62, 89, 0.75);
    font-size: 40px;
    font-weight: 600;
  }
  .advantages-list {
    display: flex;
    flex-direction: column;
    gap: 6px;
  }
  .advantages-section {
    background-color: #EFF1FD;
    margin: 0;
  }
</style>

