<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "./components/HelloWorld.vue";
import CalComponents from "./components/CalComponents.vue";
</script>

<template>
  <div>
    <CalComponents></CalComponents>
    <!--ดึงมาวางซ้ำกันหลายตัว ใส่แค่
  <CalComponents />
  <CalComponents />
  <CalComponents />-->
  </div>
</template>

<style scoped></style>
