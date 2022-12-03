<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "./components/HelloWorld.vue";
import CalComponents from "./components/CalComponents.vue";
import HelloWorldExsample from "./components/HelloWorldExsample.vue";
import HandingUserInput from "./components/HandingUserInput.vue";
import AttributeBindings from "./components/AttributeBindings.vue";
</script>

<template>
  <div>
    <AttributeBindings />
    <HandingUserInput />
    <CalComponents />
    <HelloWorldExsample />
  </div>
</template>

<style scoped>

</style>
