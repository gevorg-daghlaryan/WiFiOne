<template>
<section class="ideas mb-5">
<div class="container">
  <div class="row align-items-center ">
    <div class="col-sm-4 d-none d-lg-block">
      <img src="../../assets/images/about-us/man.png" alt="man" class="ideas-man">
    </div>
    <div class="mt-5 col-sm-8">
      <h1 class="ideas-title mb-3">We’re in The Business of Hosting Great Ideas.</h1>
      <p class="ideas-text">"To empower businesses with performant, secure, and affordable <br> managed WiFi and network solutions, enabling them to thrive in the
        <br> connected world"</p>
    </div>
  </div>
</div>
</section>
</template>
<script>
export default {
  name: 'Ideas'
}
</script>
<style>
  .ideas-title {
    color: #343E59;
    text-align: center;
    font-size: 32px;
    font-weight: 400;
  }
  .ideas {
    background-color: #F0F2FD;
    padding: 48px 0;
    margin-top:50px;
    background-image: linear-gradient(to right, #F0F2FD, #FFFFFF);
  }
  .ideas-text {
    color: #343E59;
    text-align: center;
    font-size: 19px;
    font-weight: 400;
  }
  .ideas-man {
    position: absolute;
    bottom: -165px;
  }
</style>
