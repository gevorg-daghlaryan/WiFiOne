<template>
  <div class="main-content">
    <Hero/>
<!--    <AboutUs/>-->
<!--    <ContactUs/>-->
    <Services/>
    <ChooseUs/>
    <Counter/>
    <Testimonial/>
<!--    <Works/>-->
<!--    <Support/>-->
<!--    <Accordion/>-->
    <Footer />
  </div>
</template>

<script>

import Hero from '../../components/Services/Hero.vue';
import Footer from '../../components/Services/Footer';
import AboutUs from '../../components/Services/AboutUs.vue';
import ContactUs from '../../components/Services/ContactUs.vue';
import Services from '../../components/Services/Services.vue';
import Works from '../../components/Services/Works.vue';
import Support from '../../components/Services/Support.vue';
import { themes } from '../../assets/app/app';
import Accordion from "~/components/Services/Accordion.vue";
import ChooseUs from "~/components/Services/ChooseUs.vue";
import Counter from "~/components/Services/Counter.vue";
import Testimonial from "~/components/Services/Testimonial.vue";
export default {
  layout: 'Services',
  components: {
    Testimonial,
    Counter,
    ChooseUs,
    Accordion,
    AboutUs,
    Hero,
    ContactUs,
    Services,
    Works,
    Support,
    Footer,
  },
  head() {
    return {
      title: 'High-performance WiFi Services | wifiOne',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'wifiOne services - managed WiFi and networks, event WiFi solutions, managed cameras and access systems, site power monitoring, managed media wall, etc'
        }
      ],
    }
  },
  mounted () {
    setTimeout(function () {
      themes.index()
    }, 1000)
  }
}
</script>
