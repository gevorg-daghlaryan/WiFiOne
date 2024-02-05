<template>
  <div class="image-loading">
    <div class="image-loading-center">
<!--      <img :src="require('../../assets/images/loader.gif')" alt="loader">-->
      <h1>Loading...</h1>
    </div>
  </div>
</template>
<script>
export default {
  name: 'ImageLoader'
}
</script>
<style>
  .image-loading {
    position: absolute;
    height: 100%;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .image-loading-center {
    background-color: inherit;
  }
</style>
