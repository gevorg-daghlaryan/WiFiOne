<template>
  <div>
    <p class="footer-logo"><img :src="sectionImage" width="160" alt="#"></p>
    <p class="footer-logo">{{ sectionText }}</p>
    <ul class="info-share d-inline list-inline">
      <li class="list-inline-item"><a href="#"><i class="fab fa-facebook-f" style="color: #3F81D1"></i></a></li>
      <li class="list-inline-item"><a href="#"><i class="fab fa-twitter" style="color: #3F81D1"></i></a></li>
      <li class="list-inline-item"><a href="#"><i class="fab fa-instagram" style="color: #3F81D1"></i></a></li>
    </ul>
  </div>
</template>
<script>
export default {
  name: 'FooterLogo',
  // eslint-disable-next-line vue/require-prop-types
  props: ['sectionImage', 'sectionText']
}
</script>
