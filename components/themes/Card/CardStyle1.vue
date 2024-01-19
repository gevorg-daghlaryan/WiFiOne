<template>
  <div class="card-wrapper">
    <div class="service-box d-inherit p-4 my-3 wow fadeInUp text-left">
      <slot name="cardMedia" />
      <div class="service-detail align-self-center">
        <slot name="cardTitle" />
        <slot name="cardBody" />
        <slot name="cardList" />
        <slot name="cardInfo" />
        <slot name="cardLink" />
      </div>
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
