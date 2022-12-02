<script setup lang="ts">
import { reactive, computed } from "vue";

const state = reactive({
  num1: "1",
  num2: "1",
  result: 2,
});
const result = computed(function () {
  return parseInt(state.num1) + parseInt(state.num2);
});
const doAdd = function () {
  state.result = parseInt(state.num1) + parseInt(state.num2);
};
</script>

<template>
  <div class="card">
    <div>
      <input type="text" ref="num1" v-model="state.num1" class="center_text" />
    </div>
    <div class="center_text bold_text">+</div>
    <div>
      <input type="text" ref="num2" v-model="state.num2" class="center_text" />
    </div>
    <div><button class="center_text w100px" @click="doAdd()">=</button></div>
    <div class="center_text" ref="result">{{ state.result }}</div>
    <div>{{ state.num1 }} + {{ state.num2 }} = {{ state.result }}</div>
  </div>
</template>

<style>
.center_text {
  text-align: center;
  font-size: 20pt;
  margin: 10px;
}

.bold_text {
  font-weight: bold;
}

.card {
  pading: 25px;
  background-color: rgb(228, 93, 116);
  border-style: outset;
  width: 400px;
  text-align: center;
}

.w100px {
  width: 100px;
}
</style>
