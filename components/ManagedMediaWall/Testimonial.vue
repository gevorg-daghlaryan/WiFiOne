<template>
  <section class="position-relative overview-block-ptb iq-pb-70 xamin-custom-bg">
    <div class="container">
      <div class="row">
        <div class="col-sm-12 wow fadeInUp">
          <div class="title-box wow fadeInUp text-center">
            <span class=" testimonial-title">TESTIMONIAL</span>
            <h3>1000+ people are connected through wifiOne's solutions</h3>
            <span>Unparalleled WiFi Solutions, Praised by Our Customers</span>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-md-12  wow fadeInUp">
          <div
            class="owl-carousel our-testimonial owl-loaded owl-drag"
            data-dots="true"
            data-nav="false"
            data-autoplay="false"
            data-loop="true"
            data-items="1"
            data-items-laptop="1"
            data-items-tab="1"
            data-items-mobile="1"
            data-items-mobile-sm="1"
            data-margin="30"
          >
            <div v-for="(item, index) in list" :key="index" class="item text-center">
              <div class="iq-testimonial">
                <img src="../../assets/images/testimonials/mark.png" alt="mrk" class="w-auto mx-auto">
                <p>{{ item.description }}</p>
                <div class="testimonial-info">
                  <div class="d-flex justify-content-end">
                    <img alt="#" class="img-fluid rounded-circle" :src="item.image">
                    <div class="testimonial-name d-flex flex-column">
                      <h5>{{ item.title }}</h5>
                      <span class="sub-title"> {{ item.subtitle }}</span>
                      <p class="work-name">{{item.work}}</p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: 'Testimonial',
  data () {
    return {
      list: [
        {
          title: 'Eden Dang',
          subtitle: 'Hotel Manager',
          work: '',
          description: 'Hotel Xoai engaged wifiOne to setup and manage the hotel guest and operations network. After initial setup, issues were quickly resolved with older cabling. The WiFi was carefully tuned to give reliable coverage in all areas. This enabled the hotel to focus on business operations with no downtime.',
          image: require('../../assets/images/testimonials/1.png')
        },
        {
          title: 'Mario Behling',
          subtitle: 'Business Advisor',
          work: '',
          description: 'wifiOne has been supporting the FOSSASIA OpenTech conference in Singapore during its annual summit over the last 7 years. The conference spans multiple days, attracting over 1000 attendees per day.\n' +
            'The largest deployment was 18 access points with over 550 users spanning 13 rooms; this enabled attendees real-time communications, interactive workshops and seamless connectivity throughout over all their devices.',
          image: require('../../assets/images/testimonials/2.png')
        },
        {
          title: 'Zali Rohani',
          subtitle: 'Operation Manager',
          work: 'The Working Capitol',
          description: '“WifiOne came in to resolve WiFi problems at our main campus. Over a period, they not only addressed issues with aging infrastructure but they deployed new high-spec access points with a low-cost opEx model to work with our cashflow. Not only this resolved our WiFi dropouts and coverage issues, but improved performance for smooth video calling during busy periods, offloading our staff and allowing us to scale.”',
          image: require('../../assets/images/testimonials/3.png')
        },
        {
          title: 'Patrick Tayah',
          subtitle: 'General Manager',
          work: 'The Working Capitol',
          description: 'In 2019, a major co-working space player in central Singapore was looking to modernize their communications infrastructure, at the same time reduce the Total Cost of Ownership.\n' +
            'After evaluating various solutions, wifiOne was selected as the partner. Due to the success, this was scaled to 20 sites, delivering robust and secure managed WiFi and networks to over 34 businesses 24/7.\n' +
            'Want to collaborate or have a partnership proposal? Let’s discuss it!',
          image: require('../../assets/images/testimonials/4.png')
        },
        {
          title: 'Marc Blair',
          subtitle: 'Group Head of Information ',
          work: 'Management & Strategy',
          description: '“Contrary to popular belief, Lorem Ipsum is not simply random text. It has roots in a piece of classical Latin literature from 45 BC, making it over 2000 years old.”',
          image: require('../../assets/images/testimonials/5.png')
        }
      ]
    }
  }
}
</script>
<style>
.testimonial-title {
  color: #3F81D1;
  text-align: center;
  font-size: 30px;
  font-style: normal;
  font-weight: 600;
  line-height: normal;
}
.sub-title {
  font-size: 16px;
  font-weight: 400;
}
.work-name {
  font-weight: 600;
  font-size: 16px;
  color: #71788B;
}

@media only screen and (max-width: 700px) {
  .iq-testimonial {
    padding-left: 10px !important;
    padding-right: 10px !important;
  }
}
</style>
