<template>
  <div class="xamin-blue-bg py-5 counter-section">
    <div class="container">
      <div class="row">
        <div class="col-md-6 col-lg-4 mb-3 mb-md-0">
          <div class="iq-timer style1 text-center">
            <div class="timer-details">
              <span class="timer" data-to="21" data-speed="15000">21</span>
              <p> SITES</p>
            </div>
          </div>
        </div>
        <div class="col-md-4 col-lg-4 mb-3 mb-md-0">
          <div class="iq-timer style1 text-center">
            <div class="timer-details">
              <span class="timer" data-to="146" data-speed="15000">146</span>
              <p>INFRASTRUCTURE DEVICES</p>
            </div>
          </div>
        </div>
        <div class="col-md-6 col-lg-4 mb-3 mb-md-0">
          <div class="iq-timer style1 text-center">
            <div class="timer-details">
              <span class="timer" data-to="1000" data-speed="15000">1000</span>
              <i class="fa fa-plus" aria-hidden="true" />
              <p>DEVICES</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
  export default {
    name: 'Counter'
  }
</script>
<style>
  .counter-section {
      background-image: url("/assets/images/home/bg2.svg");
      background-repeat: repeat-y;
      background-size: 651px 787px;
      background-position-y: center;
      background-position-x: 91px;
  }
</style>
