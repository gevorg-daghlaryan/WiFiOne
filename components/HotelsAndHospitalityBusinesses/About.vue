<template>
  <section class="hotel-hospital-about">
    <div class="container">
      <div class="hotel-hospital-about-wrapper">
        <img src="../../assets/images/customers/office-2.png" alt="">
        <h2 class="hotel-hospital-about-title">HOSPITALITY BUSINESSES</h2>
        <p class="hotel-hospital-about-text">
          Transform your hotel, mall, cafe, or restaurant with wifiOne's comprehensive WiFi and network solutions.
          <br>
          <br>
          Our services seamlessly integrate with existing equipment to elevate your guest experience whilst reducing your costs to align with your revenue stream. Alternatively, wifiOne can design your network before your launch.
          <br>
          <br>
          From using trusted US enterprise equipment, secure network design with the latest security standards, to data prioritization, wiifOne will support your hospitality operations.
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
.hotel-hospital-about-wrapper {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 20px;
}

.hotel-hospital-about-text {
  color: rgba(52, 62, 89, 0.75);
  font-size: 19px;
  line-height: 35px;
  font-weight: 400;
  text-align: center;
}

.hotel-hospital-about-title {
  font-size: 30px;
  font-weight: 600;
  color: #3F81D1;
}

.hotel-hospital-about {
  padding-bottom: 0;
}
</style>
