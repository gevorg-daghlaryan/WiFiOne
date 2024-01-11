<template>
  <section class="choose">
    <div class="container">
      <h2  class="text-center choose-title mb-5">WHY CHOOSE US</h2>
      <div class="row">
        <div class="col-lg-6 col-md-6" v-for="(list,index) in items" :key="index">
          <div>
            <span class="title">{{list.title}}</span>
            <p class="choose-text">{{list.description}}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: 'ChooseUs',
  data() {
    return{
      items : [
        {
          title: 'Zero upfront costs',
          description: 'Affordable running costs, aligned with your revenue model',
        },
        {
          title: 'Deployment and configuration',
          description: 'Most equipment wired, using professional equipment trusted by large enterprises',
        },
        {
          title: 'Professional network design & service',
          description: 'Giving you increased security, reliability and performance the best network is one you never notice',
        },
        {
          title: 'Single point of contact',
          description: 'Off-site and on-site top-down diagnosis in a timely manner system powered on, on-network, connection quality, actively transferring data, next steps',
        },
      ]
    }
  }
}
</script>
<style>
.title {
  color: #3F81D1;
  font-size: 24px;
  font-weight: 400;
}
.choose {
  padding-top: 0px;
}
.choose-title {
  color:#3F81D1;
  font-size: 30px;
  font-style: normal;
  font-weight: 600;
}
.choose-text {
  color: #343E59;
  font-size: 24px;
  font-weight: 400;
}
</style>
