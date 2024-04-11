<script setup>
import { onMounted, ref } from "vue"

let a = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
let sss = ref()

onMounted(() => {
  setTimeout(() => {
    a.forEach(item => {
      sss.value.style.transform = `translate(0,-${item * 10}%)`;

    });
  }, 500);
})
</script>
<template>
  <div class="kuang">
    <div ref="sss" class="sssss">
      <div v-for="(item, index) in a" :key="index" v-text="item"></div>
    </div>
  </div>
  <div class="bar">
    <div class="barnei">
      <div v-for="(item, index) in a " :key="index">
      </div>
    </div>
  </div>
</template>

<style>
.bar {
  height: 30px;
  width: 300px;
  border: 1px solid black;
  border-radius: 20px;
  display: flex;
  align-items: center;

}

.barnei {
  height: 28px;
  margin-left: 10px;
  width: 50%;
  background: linear-gradient(to right, #ffd65c, #fd7d20);
  display: flex;

}

.barnei>div {
  width: 30px;
  height: 30px;
  border-right: 1px solid white;
}

.kuang {
  width: 50px;
  height: 50px;
  background-color: aquamarine;
  overflow: hidden;
}

.sssss {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  transition: all 4s linear;
  transform: translate(0, 0);
}

/* .sssss:hover {
  transform: translate(0, -300px);

} */

.kuang>div {
  line-height: 50px;
  width: 50px;

}
</style>
