<template>
  <div class="equipment">
    <div class="list">
      <div class="list-item" v-for="(item, key) in list" :key="key">
        <img :src="item.src" alt="">
        <div class="content">
          <span>
            {{item.text}}
          </span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import img from  '../assets/production.jpg'
export default {
  name: "Equipment",
  data() {
    return {
      list: [
        {
          src: img,
          text: "ttt",
        },
        {
          src: img,
          text: "Brakes",
        },
        {
          src: img,
          text: "Brakes",
        },
        {
          src: img,
          text: "Brakes",
        },
      ],
    };
  },
};
</script>

<style scoped >
.equipment {
  margin: 100px 0;
}
.list-item {
  position: relative;
}
.equipment .list-item .content {
  position: absolute;
  display: flex;
  justify-content: center;
  align-items: center;
  top: 0;
  left: 0;
  width: 100%;
  background: rgba(0, 0, 0, 0.3);
  height: 100%;
  font-size: 1.5rem;
  z-index: 99;
  color: #fff;
  line-height: 100%;
}
img {
  width: 100%;
  height: 100%;
}
</style>