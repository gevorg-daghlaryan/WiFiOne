<template>
  <section class="works-section">
    <div class="container">
      <div class="row mb-3">
        <div class="col-lg-12">
          <div class="title-box wow fadeInUp text-center">
            <h1 class="">How wifiOne Works</h1>
          </div>
        </div>
      </div>
    </div>
    <CardsByStep/>
  </section>
</template>
<script>
import CardStyle1 from '../themes/Card/CardStyle1'
import CardsByStep from "~/components/Services/CardsByStep.vue";
export default {
  name: 'Services',
  components: {CardsByStep, CardStyle1 },
  data() {
    return{
    }
  }
}
</script>
<style>
.works-section {
  background-color: #EFF1FD;
}
</style>
