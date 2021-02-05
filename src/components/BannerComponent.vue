<template>
  <div class="banner">
    <img src="../assets/driver.png" alt="">
    <div class="mask">
      <h3>HAIRONGTAI</h3>
      <h2>
        {{'Tips For Warming Up Your Car in the Winter'.toUpperCase()}}
      </h2>
    </div>
    <!-- <div class="az-hero__headers">
          <p class="az-hero__subheader">Seasonal</p>
          <h2 class="az-hero__header">Tips For Warming Up Your Car in the Winter</h2>
        </div> -->
  </div>
</template>

<script>
export default {
  name: "BannerComponent",
};
</script>

<style scoped >
.banner {
  position: relative;
  margin-top: 40px;
}
img {
  display: block;
  width: 100%;
}
.mask {
  width: 100%;
  position: absolute;
  top: 0;
  height: 100%;
  left: 0;
  z-index: 99;
  background: rgba(0, 0,0, .5);
  color: #fff;
  text-shadow: 0 0 5px #000;
}
h2 {
  position: absolute;
  bottom: 20px;
  left: 100px;
  font-size: 2.5rem;
}
h3 {
  position: absolute;
  bottom: 380px;
  font-size: 1.5rem;
  left: 100px;
}
</style>