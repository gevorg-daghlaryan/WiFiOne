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
import Analytics from '~/components/EventWiFi/Analytics'
import Footer from '~/components/EventWiFi/Footer'
import Hero from '~/components/EventWiFi/Hero.vue'
import { themes } from '../../assets/app/app'
import Advantages from "~/components/EventWiFi/Advantages.vue";
import Counter from "~/components/EventWiFi/Counter.vue";
import Testimonial from "~/components/EventWiFi/Testimonial.vue";
import ContactUs from "~/components/EventWiFi/ContactUs.vue";
export default {
  layout: 'Services',
  components: {
    Testimonial,
    Counter,
    Advantages,
    ContactUs,
    Analytics,
    Hero,
    Footer
  },
  head() {
    return {
      title: 'Event WiFi | wifiOne',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'wifiOne brings event WiFi solutions to events of all sizes. We specialize in providing secure, fast, and reliable connectivity-ideal or indoor and outdoor events.'
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
