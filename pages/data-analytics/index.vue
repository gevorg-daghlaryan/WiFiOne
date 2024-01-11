<template>
  <div class="main-content">
<!--    <BreadCrum />-->
    <Hero/>
    <Analytics />
    <Footer />
  </div>
</template>

<script>
// import BreadCrum from '~/components/ManagedWiFI/BreadCrum'
import Analytics from '~/components/ManagedWiFI/Analytics'
import Footer from '~/components/ManagedWiFI/Footer'
import Hero from '~/components/ManagedWiFI/Hero.vue'
import { themes } from '../../assets/app/app'
export default {
  layout: 'Services',
  components: {
    // BreadCrum,
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
