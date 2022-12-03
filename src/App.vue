<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "./components/HelloWorld.vue";
import CalComponents from "./components/CalComponents.vue";
import HelloWorldExsample from "./components/HelloWorldExsample.vue";
import HandingUserInput from "./components/HandingUserInput.vue";
</script>

<template>
  <div>
    <HandingUserInput />
    <CalComponents />
    <HelloWorldExsample />
  </div>
</template>

<style scoped></style>
