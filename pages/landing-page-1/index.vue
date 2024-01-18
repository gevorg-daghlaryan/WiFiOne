<template>
  <div>
    <div class="main-content">
      <Home />
      <Business/>
      <ChooseUs />
      <Counter />
      <Services />
      <Testimonial />
      <Client />
      <ContactUs />
      <Form />
      <ContactUs1/>
    </div>
    <Footer />
  </div>
</template>

<script>
import Counter from '../../components/LandingPage1/Counter.vue';
import Home from '../../components/LandingPage1/Home.vue';
import Testimonial from '../../components/LandingPage1/Testimonial';
import ContactUs from '../../components/LandingPage1/ContactUs.vue';
import ContactUs1 from '../../components/LandingPage1/ContactUs1.vue';
import Services from '../../components/LandingPage1/Services.vue';
import Footer from '../../components/LandingPage1/Footer';
import { themes } from '../../assets/app/app';
import Business from "~/components/LandingPage1/Business.vue";
import ChooseUs from "~/components/LandingPage1/ChooseUs.vue";
import Client from "~/components/LandingPage1/Client.vue";
import Form from "~/components/LandingPage1/Form.vue";
export default {
  layout: 'LandingPage1',
  components: {
    Client,
    ChooseUs,
    Business,
    Home,
    Form,
    ContactUs,
    Counter,
    Services,
    Testimonial,
    ContactUs1,
    Footer
  },
  head() {
    return {
      title: 'Managed WiFi and Network Solutions',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Reliable, high-performance networking tailored to your business needs. Experience seamless connectivity with our managed WiFi and network solutions'
        }
      ],
    }
  },
  mounted () {
    document.cookie = 'layout=LandingPage1'
    setTimeout(function () {
      themes.index()
      themes.initRevSlider19()
    }, 1000)
  }
}
</script>
