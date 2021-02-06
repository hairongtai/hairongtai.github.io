<template>
  <div id="app">
    <div class="container">
      <SvgComponent />
      <BannerComponent />
      <ProductComponet />
      <Equipment />
      <FooterComponent />
    </div>
  </div>
</template>

<script>
import SvgComponent from "./components/SvgComponent.vue";
import ProductComponet from "./components/ProductComponet.vue";
import Equipment from "./components/Equipment.vue";
import BannerComponent from "./components/BannerComponent.vue"
import FooterComponent from './components/FooterComponent.vue'
export default {
  name: "App",
  components: {
    SvgComponent,
    ProductComponet,
    Equipment,
    BannerComponent,
    FooterComponent 
  },
};
</script>

<style>
</style>
