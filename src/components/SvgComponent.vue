<template>
  <div class="svg">
    <img src="../assets/logo.png" style="height: 100px" alt="">
    <p>HAIRONGTAI</p>
  </div>
</template>

<script>
export default {
  name: "SvgComponent",
};
</script>

<style scoped >
.svg {
  display: flex;
  justify-content: space-between;
}
/* button {
  font-size: 2rem;
} */
p {
  margin: 0;
  padding: 0;
  line-height: 6rem;
  font-size: 1.5rem;
  font-weight: bold;
  color: #221b1b;
}
</style>