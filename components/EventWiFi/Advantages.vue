<template>
  <section class="event-section">
    <div class="container">
      <div class="row">
        <div class="col-lg-8 col-sm-12 sidebar-service-left">
          <h1 class="advantages-title mb-3">Unique Advantages</h1>
          <ul class="advantages-list">
            <li>Unwavering Network Performance</li>
            <li>Enterprise-Grade Security</li>
            <li>Adaptability and Versatility</li>
            <li>Proactive Monitoring and Management</li>
            <li>Detailed Reporting and Analytics</li>
            <li>24/7 Expert Support</li>
          </ul>
        </div>
        <div class="col-lg-4 col-sm-12 pt-5 pt-lg-0">
          <img src="../../assets/images/services/event-wifi.png" alt="">
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
  .event-section {
    background-color: #EFF1FD;
    margin: 0;
  }
</style>

