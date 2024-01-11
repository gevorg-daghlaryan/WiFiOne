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
import Analytics from '~/components/MamagedCameras/Analytics'
import Footer from '~/components/MamagedCameras/Footer'
import Hero from '~/components/MamagedCameras/Hero.vue'
import { themes } from '../../assets/app/app'
import ContactUs from "~/components/MamagedCameras/ContactUs.vue";
import Advantages from "~/components/MamagedCameras/Advantages.vue";
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
