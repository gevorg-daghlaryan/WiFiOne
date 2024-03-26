<template>
  <div class="main-content">
    <Hero/>
    <Customer/>
    <ChooseUs/>
    <Counter/>
    <Studies/>
    <Client/>
    <ContactUs/>
    <Footer/>
  </div>
</template>
<script>
  import { themes } from "~/assets/app/app";
  import Hero from "~/components/Customers/Hero.vue";
  import Customer from "~/components/Customers/Customer.vue";
  import ContactUs from "~/components/Customers/ContactUs.vue";
  import ChooseUs from "~/components/Customers/ChooseUs.vue";
  import Studies from "~/components/Customers/Studies.vue";
  import Footer from "~/components/Customers/Footer.vue";
  import Counter from "~/components/Customers/Counter.vue";
  import Client from "~/components/Customers/Client.vue";
  export default {
    layout: 'Pages',
    components: {
      Client,
      Counter,
      Footer,
      Studies,
      ChooseUs,
      ContactUs,
      Hero,
      Customer,
    },
    head() {
      return {
        title: 'Clients | wifiOne',
        meta: [
          {
            hid: 'description',
            name: 'description',
            content: 'The spectrum of wifiOne clientele ranges from offices and businesses to event companies, hotels, restaurants, and more. We deliver seamless, reliable connectivity. '
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
