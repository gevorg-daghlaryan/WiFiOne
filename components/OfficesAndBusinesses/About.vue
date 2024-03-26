<template>
  <section class="customers-office-and-business-about">
    <div class="container">
      <div class="office-and-business-wrapper">
        <img src="../../assets/images/customers/office-1.png" alt="">
        <h2 class="customers-office-and-business-about-title">OFFICE-BASED BUSINESSES</h2>
        <p class="customers-office-and-business-about-text">Enjoy no upfront costs, aligned with your business revenue model. Our seasoned engineers employ industry best practices, conducting thorough site surveys and logical network designs tailored to your objectives. Installation is seamless, with certified engineers configuring and validating equipment. Our offerings include top-tier routers and access points from leading US and European manufacturers, ensuring separation of concerns and WPA3 wireless security. Monthly software updates and network vulnerability auditing options maintain peak performance and security.
          <br><br>
          Tailor your brand with a custom portal, appearing upon user connection, while shared office spaces benefit from per-tenant networks, optimal separation, and secure one-way access to shared devices. Enjoy network fairness with Quality of Service, resource abuse prevention, and smooth video calling even during heavy media traffic. Choose wifiOne for smart business value, professional network design, and secure, optimized connectivity.
        </p>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name:'About'
}
</script>
<style>
  .office-and-business-wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 20px;
  }
  .customers-office-and-business-about-text {
    color: rgba(52, 62, 89, 0.75);
    font-size: 20px;
    line-height: 35px;
    font-weight: 400;
    text-align: center;
  }
  .customers-office-and-business-about-title {
    font-size: 30px;
    font-weight: 600;
    color: #3F81D1;
  }
  .customers-office-and-business-about {
    padding-bottom: 0;
  }
</style>
