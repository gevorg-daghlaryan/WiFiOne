<template>
  <section class="event-management-about">
    <div class="container">
      <div class="event-management-about-wrapper">
        <img src="/assets/images/customers/office-2.png" alt="">
        <h2 class="event-management-about-title">EVENT MANAGEMENT COMPANIES</h2>
        <p class="event-management-about-text">
          Our service ensures a seamless experience for your attendees, with smooth voice/video calling thanks to the wire-free 5G technology.
          <br>
          <br>
          Our dedicated team of engineers will remotely configure the experience you want to deliver, allowing you to present multiple WiFi networks with optional advertising portals, so deliver WiFi for your attendees and support your event staff and point of sale systems.
          <br>
          <br>
          You just need to place the equipment. Smart, cost-effective billing means you will be invoiced only for days the equipment is used.
        </p>
      </div>
    </div>
  </section>
</template>
<script>
  export default {
    name: 'About'
  }
</script>
<style>
  .event-management-about-wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 20px;
  }

  .event-management-about-text {
    color: rgba(52, 62, 89, 0.75);
    font-size: 19px;
    line-height: 35px;
    font-weight: 400;
    text-align: center;
  }

  .event-management-about-title {
    font-size: 30px;
    font-weight: 600;
    color: #3F81D1;
  }

  .event-management-about {
    padding-bottom: 0;
  }
</style>
