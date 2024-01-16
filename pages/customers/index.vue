<template>
  <div class="main-content">
    <Hero/>
    <Customer/>
    <ContactUs/>
    <ChooseUs/>
    <Testimonial/>
    <Studies/>
    <ContactUs1/>
    <Footer/>

  </div>
</template>
<script>

import { themes } from '../../assets/app/app';
import Hero from '../../components/Customers/Hero.vue'
import Customer from '../../components/Customers/Customer.vue'
import ContactUs from "~/components/Customers/ContactUs.vue";
import ChooseUs from "~/components/Customers/ChooseUs.vue";
import Testimonial from "~/components/Customers/Testimonial.vue";
import Studies from "~/components/Customers/Studies.vue";
import Footer from "~/components/Customers/Footer.vue";
import ContactUs1 from "~/components/Customers/ContactUs1.vue";
export default {
  layout: 'Pages',
  components: {
    ContactUs1,
    Footer,
    Studies,
    Testimonial,
    ChooseUs,
    ContactUs,
    Hero,
    Customer,
  },
  mounted () {
    setTimeout(function () {
      themes.index()
    }, 1000)
  }
}
</script>
