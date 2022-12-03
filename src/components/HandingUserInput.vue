<script setup lang="ts">
import { ref } from "vue";
const message = ref("Hello World!");
function reverseMessage() {
  message.value = message.value.split("").reverse().join(""); //กลับซ้ายขวา หน้าหลัง แยกร่าง
}
function notify() {
  alert("navigation was prevented");
}
</script>

<template>
  <h1>{{ message }}</h1>
  <button @click="reverseMessage">Reverse Message</button>
  <button v-on:click="message += '!'">Append "!"</button>
  <a href="https://vuejs.org" @click.prevent="notify"
    >A link with e.preventDefault</a
  >
  <!--prevent ไม่ให้เปิดลิงค์-->
</template>

<style scoped>
button,
a {
  display: block;
  margin-bottom: 1em;
}
</style>
