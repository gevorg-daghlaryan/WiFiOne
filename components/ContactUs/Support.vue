
<template>
  <section  class="xamin-blue-bg pt-5 pb-5">
    <div class="container">
          <div class="w-100 mt-3 d-flex  justify-content-center align-items-center flex-wrap support-wrapper">
            <img src="../../assets/images/contact-us/Time.svg" alt="">
            <h6 class="description text-white">Get same-day equipment replacement and easy <br> reconfiguration for your changing needs</h6>
            <button
              id="submit-4"
              click="/contact-us"
              name="submit"
              type="submit"
              value="Send"
              class="button  white-btn mt-3 form-button"
            >
              Submit support ticket
            </button>
        </div>
    </div>
  </section>
</template>
<script>
export default {
  name: 'Support',
}
</script>
<style>
  .description {
    font-size: 30px;
    font-weight: 600;
  }
  .form-button {
    font-size: 14px;
  }
  .support-wrapper {
    gap: 30px;
  }
  .support-wrapper {
    gap: 30px;
  }
</style>
