<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-sm-12">
          <div class="iq-accordion career-style about-style">
            <div v-for="(item,index) in items" :key="index" class="iq-accordion-block">
              <div class="active-faq clearfix">
                <div class="container">
                  <div class="row ">
                    <div class="col-md-12 col-sm-12">
                      <a href="javascript:void(0)" class="accordion-title"><span>{{ item.title }}</span></a>
                    </div>
                  </div>
                </div>
              </div>
              <div class="accordion-details">
                <div class="container">
                  <div class="row mt-4 w-100  ml-4">
                    <p class="accordion-description">{{item.description}}</p>
                  </div>
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
  name: 'Accordion',
  data () {
    return {
      items: [
        {
          title: 'Can You Integrate With Existing Networks?',
          description: 'Yes, either we can place our network equipment upstream of yours, or integrate to your existing network if preferred',
        },
        {
          title: 'What Are Your Support Points Of Contact?',
          description: 'We offer realtime support via WhatsApp messaging and calling, as well as form submission and email',
        },
        {
          title: 'What Differentiates You From The Competitors?',
          description: 'wifiOne uses best-in-class enterprise equipment to offer optimal reliability and performance for cost-senstive markets',
        },
        {
          title: 'How Can You Achieve Better Pricing Than The Competition?',
          description: 'wifiOne has a lean structure of experts, enabled by cloud automation and proven configurations; this allows attention to be spent where it makes the most difference',
        },
        {
          title: 'Can Your Networks Be Customised To Integrate Existing Systems?',
          description: 'Yes, during early consultation, network experts will identify any existing equipment requirements and design this into the final solution',
        },
        {
          title: 'How Does Your WiFi And Networks Improve My Security?',
          description: 'How does your WiFi and networks improve my security?',
        },
      ],
    }
  },
  mounted () {
    const jquery = window.$
    jQuery('.iq-accordion .iq-accordion-block .accordion-details').hide()
    // jQuery('.iq-accordion .iq-accordion-block:first').addClass('accordion-active').children().slideDown('slow')
    jQuery('.iq-accordion .iq-accordion-block').on('click', function () {
      jQuery('.iq-accordion .iq-accordion-block').not(this).removeClass('accordion-active').children('div.accordion-details ').slideUp('slow');
      jQuery(this).toggleClass('accordion-active').children('div.accordion-details ').slideToggle('slow');
    })
  }
}
</script>
<style  scoped>
  .accordion-title:before {
    background: transparent !important;
    color: #3F81D1 !important;
    box-shadow: none !important;
    font-size: 30px;
  }
  .accordion-description {
    color: #343E59;
    font-size: 18px;
    font-style: normal;
    font-weight: 400;
    text-transform: capitalize;
  }
</style>
