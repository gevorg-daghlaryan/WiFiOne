<template>
  <section class="choose">
    <div class="container">
      <h2  class="text-center choose-header mb-5">WHY CHOOSE US</h2>
      <div class="choose-wrapper">
        <div class="choose-item" v-for="(list,index) in items" :key="index">
          <img :src="list.img" alt="" class="d-block">
          <div class="">
            <span class="choose-title">{{list.title}}</span>
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
          img: '/images/home/choose-us/1.svg'
        },
        {
          title: 'Professional network design & service',
          description: 'Giving you increased security, reliability and performance the best network is one you never notice',
          img: '/images/home/choose-us/2.svg'

        },
        {
          title: 'Deployment and configuration',
          description: 'Most equipment wired, using professional equipment trusted by large enterprises',
          img: '/images/home/choose-us/3.svg'
        },
        {
          title: 'Single point of contact',
          description: 'Off-site and on-site top-down diagnosis in a timely manner system powered on, on-network, connection quality, actively transferring data, next steps',
          img: '/images/home/choose-us/4.svg'
        },
      ]
    }
  }
}
</script>
<style>
  .choose-wrapper {
    min-height: 100%;
    display: flex;
    flex-wrap: wrap;
    flex-direction: row;
    justify-content: space-between;
  }
  .choose-item {
    display: flex;
    flex-basis: 45%;
    justify-content: center;
    align-items: start;
    gap: 20px
  }
  .choose-title {
    color: #3F81D1;
    font-size: 24px;
    font-weight: 400;
    margin-bottom: 10px;
  }
  .choose {
    background-color: #EFF1FD ;
  }
  .choose-header {
    color: #3F81D1;
    font-size: 30px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    text-transform: uppercase;
  }
  .choose-text {
    color: #343E59;
    font-size: 20px;
    font-style: normal;
    margin-bottom: 50px;
  }
  @media only screen and (max-width: 600px) {
    .choose-wrapper {
      flex-direction: column;
    }
  }
</style>
