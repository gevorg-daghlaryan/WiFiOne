
  <template>
    <section  class="xamin-blue-bg pt-5 pb-5 service-support-section">
      <div class="container">
        <div class="service-support-wrapper">
          <h6 class="support-description text-white text-center">We prioritize your operational continuity, offering same-day equipment replacement.
            <br> Trust wifiOne for swift and tailored solutions that keep your business running smoothly.</h6>
          <a
            id="submit-4"
            href="/contact-us"
            class="button  white-btn mt-3 form-button mx-auto"
          >
            Contact Us
          </a>
        </div>
      </div>
    </section>
  </template>
<script>
export default {
  name: 'Support'
}
</script>
<style>
  .service-support-section {
    background-image: url("../../assets/images/home/bg2.svg");
    background-repeat: repeat-y;
    background-size: 651px 787px;
    background-position-y: center;
    background-position-x: 91px;
  }
  .service-support-wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .support-description {
    font-weight: 400;
    font-size: 29px;
  }
</style>
