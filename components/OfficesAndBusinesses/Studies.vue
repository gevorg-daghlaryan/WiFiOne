<template>
  <section>
    <h1 class="text-center studies">CASE STUDIES</h1>
    <div class="container customer-studies-container">
      <img src="../../assets/images/customers/capitol.png" alt="logo">
      <h2 class="text-center text-white studies-title">The Working Capitol</h2>
      <p class="text-center text-white studies-text">
        In 2019, a major co-working space player in central Singapore was looking to modernize their communications infrastructure, at the same time reduce the Total Cost of Ownership.
        <br>
        <br>
        After evaluating various solutions, wifiOne was selected as the partner. Due to the success, this was scaled to 20 sites, delivering robust and secure managed WiFi and networks to over 34 businesses 24/7.
      </p>
      <div class="author">
        <img src="../../assets/images/customers/avatar-2.png" alt="avatar">
        <div class="text-white">
          <h4 class="text-white author-name">Patrick Tayah</h4>
          <p class="author-text">General Manager <br> The Working Capitol</p>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
name:'Studies'
}
</script>
<style>

 .studies {
   color: #3F81D1;
   font-size: 30px;
   font-style: normal;
   font-weight: 600;
   line-height: normal;
   margin-bottom: 50px;
 }
 .customer-studies-container {
   background-image: url("../../assets/images/customers/base-bg.avif");
   background-position: center;
   background-repeat: no-repeat;
   background-size: cover;
   padding: 100px;
   display: flex;
   flex-direction: column;
   align-items: center;
   justify-content: center;
   gap: 14px;
   border-radius: 20px;
 }
 .studies-title {
   font-size: 35px;
   font-style: normal;
   font-weight: 600;
   line-height: normal;
 }
 .studies-text {
   text-align: center;
   font-size: 20px;
   font-style: normal;
   font-weight: 400;
 }
 .author {
   display: flex;
   width: 100%;
   gap: 20px;
   align-items: start;
   justify-content: end;
 }
 .author-name {
   color: #FFF;
   font-size: 20px;
   font-style: normal;
   font-weight: 600;
   line-height: normal;
   margin-bottom: 4px;
 }
 .author-text {
   font-size: 17px;
   font-style: normal;
   font-weight: 600;
   line-height: normal;
 }
 @media (max-width: 600px) {
   .customer-studies-container {
     padding: 50px 10px;
   }
 }
</style>
