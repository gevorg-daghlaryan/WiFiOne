<template>
  <section class="contact-us-top">
      <div class="container">
        <div class="contact-us-top-wrapper">
          <h1 class="text-white contact-us-top-title"> Contact Us</h1>
          <p class="text-white contact-us-top-text">We welcome your inquiries—use the form below to get in touch.</p>
        </div>
    </div>
  </section>

</template>
<script>
export default {
  name:'BreadCrump'
}
</script>
<style>
  .contact-us-top {
    background-image: url("../../assets/images/contact-us/contact-us.png");
    background-position: center;
    background-repeat: no-repeat;
    background-size:cover;
    height: 490px;
  }
  .contact-us-top-text {
    font-size: 21px;
  }
  .contact-us-top-wrapper {
    display: flex;
    flex-direction: column;
    align-items: start;
    justify-content: start;
    gap: 31px;
    height: 100%;
  }
</style>
