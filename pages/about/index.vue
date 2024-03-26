<template>
  <div>
    <div class="main-content">
      <BreadCrump/>
      <Story/>
      <Ideas/>
      <ChooseUs/>
      <Counter/>
      <Testimonial/>
      <ContactUs/>
      <Footer />
    </div>
  </div>
</template>

<script>
  import AboutUs from "~/components/AboutUs-1/AboutUs";
  import History from "~/components/AboutUs-1/History";
  import Team from "~/components/AboutUs-1/Team";
  import Footer from "~/components/AboutUs-1/Footer";
  import { themes } from "~/assets/app/app";
  import BreadCrump from "~/components/AboutUs-1/BreadCrum.vue";
  import Story from "~/components/AboutUs-1/Story.vue";
  import ChooseUs from "~/components/AboutUs-1/ChooseUs.vue";
  import Awards from "~/components/AboutUs-1/Awards.vue";
  import ContactUs from "~/components/AboutUs-1/ContactUs.vue";
  import Testimonial from "~/components/AboutUs-1/Testimonial.vue";
  import Ideas from "~/components/AboutUs-1/Ideas.vue";
  import Counter from "~/components/AboutUs-1/Counter.vue";


  export default {
    layout: 'AboutUs',
    components: {
      Ideas,
      Testimonial,
      ContactUs,
      Awards,
      ChooseUs,
      History,
      Team,
      Footer,
      BreadCrump,
      Story,
      Counter,

    },
    data () {
      return {
        links: [{
          title: 'Home',
          href: 'landing-page'
        }]
      }
    },
    head() {
      return {
        title: 'About Us | wifiOne',
        meta: [
          {
            hid: 'description',
            name: 'description',
            content: 'wifiOne is a boutique solution provider, specializing in delivering performant and secure managed WiFi and networks at an affordable price point.'
          }
        ],
      }
    },
    mounted () {
      // const layout = themes.getCookie('layout')
      // this.$nuxt.setLayout(layout)
      setTimeout(function () {
        themes.index()
      }, 1000)
    }
  }
</script>
