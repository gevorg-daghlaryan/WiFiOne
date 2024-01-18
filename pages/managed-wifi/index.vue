<template>
  <div class="main-content">
    <Hero/>
    <Analytics />
    <Advantages/>
    <ContactUs/>
    <Footer />
  </div>
</template>

<script>
import Analytics from '~/components/ManagedWiFI/Analytics'
import Footer from '~/components/ManagedWiFI/Footer'
import Hero from '~/components/ManagedWiFI/Hero.vue'
import { themes } from '../../assets/app/app'
import ContactUs from "~/components/ManagedWiFI/ContactUs.vue";
import Advantages from "~/components/ManagedWiFI/Advantages.vue";
export default {
  layout: 'Services',
  components: {
    Advantages,
    ContactUs,
    Analytics,
    Hero,
    Footer
  },
  head() {
    return {
      title: 'Managed WiFi and Networks | wifiOne',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'wifiOne provides seamless connectivity with managed WiFi and network solutions. High-quality, secure coverage and equipment layout for strong WiFi .'
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
