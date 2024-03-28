<template>
  <section class="customers">
    <div class="container">
      <h2 class="customers-title">OUR CUSTOMERS</h2>
      <div class="customers-wrapper">
        <div class="customer-item">
          <img src="../../assets/images/customers/office-based-businesses.png" alt="logo" class="customer-card-img">
          <h2 class="customer-card-title">Office-based Businesses</h2>
          <p class="customer-card-text"> Transform your office into a hub of productivity and seamless communication with wifiOne. Our tailored solutions ensure reliable and high-performance WiFi, empowering your team to collaborate efficiently and drive success.</p>
          <a  class="button  button-icon text-center" href="/offices-and-businesses">Learn More</a>
        </div>
        <div class="customer-item">
          <img src="../../assets/images/customers/office-based-businesses.png" alt="logo" class="customer-card-img">
          <h2 class="customer-card-title">Event Management Companies</h2>
          <p class="customer-card-text">Deliver exceptional experiences during events, conferences, and gatherings with wifiOne's reliable WiFi solutions. From seamless attendee connectivity to robust event management, we ensure your events run smoothly, leaving a lasting impression on participants.</p>
          <a  class="button  button-icon text-center" href="/event-management-companies">Learn More</a>
        </div>
        <div class="customer-item">
          <img src="../../assets/images/customers/office-based-businesses.png" alt="logo" class="customer-card-img">
          <h2 class="customer-card-title">Hospitality Businesses</h2>
          <p class="customer-card-text">From hotels to malls, cafes, and restaurants, elevate guest satisfaction in hospitality establishments with wifiOne. Our solutions provide guests with uninterrupted and secure connectivity, enhancing their overall experience and ensuring your business stands out in the competitive hospitality landscape.</p>
          <a  class="button  button-icon text-center" href="/hotels-and-hospitality-businesses">Learn More</a>
        </div>
      </div>
    </div>

  </section>
</template>
<script>
export default {
  name:'Customer'
}
</script>
<style>
 .customers-wrapper {
   display: flex;
   justify-content: space-between;
   gap: 30px;
 }
   .customer-item {
     display: flex;
     align-items: center;
     justify-content: space-between;
     flex-direction: column;
     background-color: #659ADA;
     border-radius: 20px;
     padding: 30px 25px;
     min-height: 460px;
     max-width: 362px;
     gap: 15px;
     box-shadow: 0px 8px 10px -5px #6CA3D9;
   }
   .customer-card-img {
     display: block;
     width: 70px;
     height: 70px;
   }
   .customer-card-title {
     font-size: 20px;
     text-align: center;
     font-weight: 600;
     color: #343E59;
   }
   .customer-card-text {
      font-size: 16px;
      font-weight: 400;
      color: white;
      text-align: center;
   }
   .customers-title {
     font-size: 30px;
     font-weight: 600;
     color: #3F81D1;
     text-align: center;
     margin-bottom: 30px;
   }

 @media only screen and (max-width: 850px) {
   .customers-wrapper {
     flex-direction: column;
     align-items: center;
   }
   ․customer-item {
     margin: 0 auto;
   }
 }

</style>
