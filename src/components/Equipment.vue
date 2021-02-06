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
import img1 from  '../assets/equipment/car1.jpg'
import img2 from  '../assets/equipment/car2.jpg'
import img3 from  '../assets/equipment/car3.jpg'
import img4 from  '../assets/equipment/car4.jpg'
export default {
  name: "Equipment",
  data() {
    return {
      list: [
        {
          src: img1,
          text: "driver",
        },
        {
          src: img2,
          text: "Brakes",
        },
        {
          src: img3,
          text: "engine",
        },
        {
          src: img4,
          text: "steering wheel",
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
  width: 1600px;
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