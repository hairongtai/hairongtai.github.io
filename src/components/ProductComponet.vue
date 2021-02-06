<template>
  <div>
    <div class="list">
      <div class="list-item" v-for="(item, key) in list" :key="key">
        <img style="width: 100%;" :src="item.src" />
        <div class="container" style="margin-top: 20px">
          <h3>
            {{item.title}}
          </h3>
          <p>
            {{item.text}}
          </p>
        </div>
      </div>
    </div>
    <div class="list">
      <div class="list-item" v-for="(item, key) in list" :key="key">
        <img style="width: 100%;" :src="item.src" />
        <div class="container" style="margin-top: 20px">
          <h3>
            {{item.title}}
          </h3>
          <p>
            {{item.text}}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import img1 from "../assets/equipment/car1.jpg";
import img2 from "../assets/equipment/car2.jpg";
import img3 from "../assets/equipment/car3.jpg";
import img4 from "../assets/equipment/car4.jpg";
export default {
  name: "ProductComponet",
  data() {
    return {
      list: [
        {
          src: img1,
          title: "How to Winterize Your Car",
          text: `Winter means bad weather, less sunlight, and poor road conditions. Luckily, a small amount of basic
            maintenance and some quick inspections can get your car ready to drive through winter weather.  `,
        },
        {
          src: img2,
          title: "How to Winterize Your Car",
          text: `Winter means bad weather, less sunlight, and poor road conditions. Luckily, a small amount of basic
            maintenance and some quick inspections can get your car ready to drive through winter weather.  `,
        },
        {
          src: img3,
          title: "How to Winterize Your Car",
          text: `Winter means bad weather, less sunlight, and poor road conditions. Luckily, a small amount of basic
            maintenance and some quick inspections can get your car ready to drive through winter weather.  `,
        },
        {
          src: img4,
          title: "How to Winterize Your Car",
          text: `Winter means bad weather, less sunlight, and poor road conditions. Luckily, a small amount of basic
            maintenance and some quick inspections can get your car ready to drive through winter weather.  `,
        },
      ],
    };
  },
};
</script>

<style>
.list {
  display: flex;
  margin-top: 200px;
  justify-content: space-between;
}

@media screen and (max-width: 480px) {
  .list {
    display: block;
  }
}
.list-item {
  margin: 0 60px;
  box-shadow: 0 1px 3px 0 rgb(32 33 36 / 12%), 0 1px 1px 0 rgb(32 33 36 / 14%),
    0 2px 1px -1px rgb(32 33 36 / 20%);
}
.list-item img {
  box-sizing: border-box;
  display: block;
  height: 1020px;
}
.list-item h3 {
  text-align: center;
  font-size: 1.5rem;
}
</style>