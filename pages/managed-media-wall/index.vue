<template>
  <div class="main-content">
    <Hero/>
    <Analytics />
    <Advantages/>
    <Counter/>
    <Testimonial/>
    <ContactUs/>
    <Footer />
  </div>
</template>

<script>
  import Analytics from "~/components/ManagedMediaWall/Analytics";
  import Footer from "~/components/ManagedMediaWall/Footer";
  import Hero from "~/components/ManagedMediaWall/Hero.vue";
  import { themes } from "~/assets/app/app";
  import ContactUs from "~/components/ManagedMediaWall/ContactUs.vue";
  import Advantages from "~/components/ManagedMediaWall/Advantages.vue";
  import Counter from "~/components/ManagedMediaWall/Counter.vue";
  import Testimonial from "~/components/ManagedMediaWall/Testimonial.vue";
  export default {
    layout: 'Services',
    components: {
      Testimonial,
      Advantages,
      ContactUs,
      Analytics,
      Hero,
      Footer,
      Counter
    },
    head() {
      return {
        title: 'Media Wall and Signage | wifiOne',
        meta: [
          {
            hid: 'description',
            name: 'description',
            content: 'wifiOne\'s Managed Media Wall and Signage service is designed to enhance communication through dynamic and effective message delivery.'
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
