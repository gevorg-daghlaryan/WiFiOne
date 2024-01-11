<template>
  <div class="main-content">
<!--    <BreadCrum />-->
    <Hero/>
    <Analytics />
    <Advantages/>
    <ContactUs/>
    <Footer />
  </div>
</template>

<script>
import Analytics from '~/components/EventWiFi/Analytics'
import Footer from '~/components/EventWiFi/Footer'
import Hero from '~/components/EventWiFi/Hero.vue'
import { themes } from '../../assets/app/app'
import ContactUs from "~/components/EventWiFi/ContactUs.vue";
import Advantages from "~/components/EventWiFi/Advantages.vue";
export default {
  layout: 'Services',
  components: {
    Advantages,
    ContactUs,
    Analytics,
    Hero,
    Footer
  },
  mounted () {
    setTimeout(function () {
      themes.index()
    }, 1000)
  }
}
</script>
