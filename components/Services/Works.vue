<template>
  <section class="aboutus-two-service">
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div class="title-box wow fadeInUp text-center">
            <span class="work-header">HOW IT WORKS</span>
            <h1 class="">How Does WiFiOne Work</h1>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-lg-4 col-md-6 h-100" v-for="(list,index) in items" :key="index">
          <CardStyle1>
            <div slot="cardMedia" class="d-flex justify-content-center mb-2">
              <img :src="list.src" alt="fancy-list" class="mx-auto">
            </div>
            <div slot="cardTitle">
              <h5 class="mb-2 text-center">{{ list.title }}</h5>
            </div>
            <div slot="cardBody">
              <p class="text-center">{{ list.description }}</p>
            </div>
          </CardStyle1>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import CardStyle1 from '../themes/Card/CardStyle1'
export default {
  name: 'Services',
  components: { CardStyle1 },
  data() {
    return{
      items : [
        {
          title: 'Site Survey',
          description: 'Site survey will be conducted to comprehensively understand coverage and equipment requirements.',
          src: require('../../assets/images/home/services/02.png')
        },
        {
          title: 'Fiber Setup',
          description: 'The business will initiate the ordering process for an internet fiber plan from the Internet Service Provider (ISP) to establish the foundation for robust connectivity.',
          src: require('../../assets/images/home/services/04.png')
        },
        {
          title: 'Installation',
          description: 'Cabling installation will be carried out to meet stringent 5GbE requirements, ensuring a high-quality and reliable network infrastructure.',
          src: require('../../assets/images/home/services/01.png')
        },
        {
          title: 'Configuration',
          description: 'New equipment will be deployed, and multiple networks will be configured to optimize performance and meet specific business needs. Existing equipment will be seamlessly integrated.',
          src: require('../../assets/images/home/services/05.png')
        },
        {
          title: 'Validation',
          description: 'Rigorous validation processes will be implemented for both new and existing equipment and networks, ensuring functionality and performance. Staff will be involved in testing.',
          src: require('../../assets/images/home/services/07.png')
        },
        {
          title: 'Monitoring',
          description: 'The commencement of infrastructure and key equipment monitoring, guaranteeing ongoing operational excellence through proactive monitoring measures.',
          src: require('../../assets/images/home/services/03.png')
        }
      ]
    }
  }
}
</script>
<style>
  .work-header {
    color: #3F81D1;
    font-size: 30px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
  }
</style>
