<template>
  <section class="advantages-section">
    <div class="container">
      <div class="row">
        <div class="col-lg-8 col-sm-12 sidebar-service-left">
          <h1 class="advantages-title mb-3">Unique Advantages</h1>
          <ul class="advantages-list">
            <li>Enhanced security</li>
            <li>Streamlined access control</li>
            <li>Real-time visibility and monitoring</li>
            <li>Expert installation and ongoing support</li>
            <li>Dedicated mobile app</li>
            <li>Smart business value</li>
          </ul>
        </div>
        <div class="col-lg-4 col-sm-12 pt-5 pt-lg-0">
          <img src="../../assets/images/services/manag-cam.png" alt="">
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

