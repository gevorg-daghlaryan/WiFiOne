<style>
.title {
  font-weight: 300;
  font-size: 20px;
}
.support-section {
  line-height: 25px;
}
.description {
  color: #343E59;
  font-size: 20px;
  font-weight: 700;
}
.support-info {
  font-weight: 400;
  font-size: 20px
}
</style>
<template>
  <section  class="xamin-blue-bg pt-5 pb-5">
    <div class="container">
          <div class="w-100 mt-3 d-flex  justify-content-between align-items-center">
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
</style>
