<template>
  <div class="card-wrapper">
    <div class="service-box  p-4 my-3 wow fadeInUp text-center d-flex flex-column ">
      <slot name="cardMedia" />
      <div class="service-detail ">
        <slot name="cardTitle" />
        <slot name="cardInfo" />
        <slot name="cardBody" />
        <slot name="cardList" />
      </div>
      <slot name="cardLink" />
    </div>
  </div>
</template>
<script>
export default {
  name: 'CardStyle1'
}
</script>
<style>
  .card-wrapper {
    height: 100%;
    margin-bottom: 10px;
  }
  .service-box {
    height: 100%;

  }
</style>
