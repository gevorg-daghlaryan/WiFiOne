<template>
  <section class="">
    <div class="container">
      <div class="row">
        <div class="col-sm-12">
          <div class="row">
            <div class="rmb-30 col-md-8">
              <h2 class="text-center text-md-left mb-3">Get a Quote Instantly</h2>
              <div>
                <div class="types">
                  <b-form-checkbox v-model="coverageOptimized">
                    Coverage-optimised WiFi +$1/sqm/mo
                  </b-form-checkbox>

                  <b-form-checkbox v-model="performanceUpgrade">
                    Performance WiFi upgrade +$1/sqm/mo
                  </b-form-checkbox>

                  <b-form-checkbox v-model="powerMonitoring">
                    Automatic power outage monitoring +$20/mo
                  </b-form-checkbox>

                  <b-form-checkbox v-model="lteBackup">
                    LTE internet backup +$50/mo
                  </b-form-checkbox>
                </div>
                <p>Square Meter</p>
                <div class="square">
                  <div class="square-number">{{ value }}</div>
                  <span>m<sup>2</sup></span>
                </div>
                <div class="ranges">
                  <div class="range-wrapper">
                    <b-form-input v-model="value" type="range" min="0" max="1000"></b-form-input>
                  </div>
                  <div class="ranges-limits">
                    <div>0 m <sup>2</sup></div>
                    <div>1000 m <sup>2</sup></div>
                  </div>
                </div>

              </div>

            </div>
            <div class="col-md-4">
              <div class="xamin-blue-bg text-white px-3 py-5">
                <h3 class="text-white">Managed Network</h3>
                <p class="text-white m-0 mb-2">Router and managment</p>
                <span class="text-white price">${{total()}}/mo</span>
                <p class="text-white m-0">Competitors $3.20</p>
                <p class="text-white m-0 font-weight-bold">Top Features</p>
                <div class="list-item">
                  <img src="../../assets/images/home/mark.png" alt="icon">
                  <span>24/7 cloud monitoring</span>
                </div>
                <div class="list-item">
                  <img src="../../assets/images/home/mark.png" alt="icon">
                  <span>Multiple support channels</span>
                </div>
                <div class="list-item">
                  <img src="../../assets/images/home/mark.png" alt="icon">
                  <span class="">Same-day equipment replacement</span>
                </div>
                <div class=" text-center mt-5 w-100">
                  <a class="button white-btn button-icon w-100" href="#"><span class="btn-effect">Get Monthly Plan</span></a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>

export default {
  name: 'Form',
  data() {
    return {
      defaultValue: 200,
      value: 0,
      coverageOptimized: false,
      performanceUpgrade: false,
      powerMonitoring: false,
      lteBackup: false,
    }
  },
  methods: {
    total() {
      return  +this.defaultValue + (+(this.coverageOptimized ? this.value : +0)) + (+(this.performanceUpgrade ? this.value : +0)) + (+(this.powerMonitoring ? +20 : +0)) + (+(this.lteBackup ? +50 : +0));
    }
  }
}
</script>
<style>
  .price {
    display: block;
    width: 100%;
    text-align: center;
    background-color: #659ADA;
    font-weight: bold;
    border-radius: 3px;
    font-size: 30px;
    padding: 5px 0;
  }
  .list-item {
    display: flex;
    align-items: center;
    gap: 10px;
  }
  .square {
    display: flex;
    gap: 5px;
    align-items: center;
    margin-bottom: 10px;
    font-size: 21px;
  }
  .square-number {
    padding: 3px 30px;
    background-color: #EFF1FD;
    border: 1px solid #AAABB4;
  }
  .ranges {
    display: flex;
    flex-direction: column;
    max-width: 650px;
  }
  .ranges-limits {
    display: flex;
    justify-content: space-between;
  }
  .types {
    display: flex;
    flex-direction: column;
    gap: 23px;
    color: #343E59;
    font-size: 25px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 40px;
  }
  .range-wrapper {

  }
</style>
