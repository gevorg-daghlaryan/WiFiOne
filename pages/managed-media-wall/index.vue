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
import Analytics from '~/components/ManagedMediaWall/Analytics'
import Footer from '~/components/ManagedMediaWall/Footer'
import Hero from '~/components/ManagedMediaWall/Hero.vue'
import { themes } from '../../assets/app/app'
import ContactUs from "~/components/ManagedMediaWall/ContactUs.vue";
import Advantages from "~/components/ManagedMediaWall/Advantages.vue";
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
