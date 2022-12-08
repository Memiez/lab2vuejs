<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "./components/HelloWorld.vue";
import CalComponents from "./components/CalComponents.vue";
import HelloWorldExsample from "./components/HelloWorldExsample.vue";
import HandingUserInput from "./components/HandingUserInput.vue";
import AttributeBindings from "./components/AttributeBindings.vue";
import ConditionsAndLoops from "./components/ConditionsAndLoops.vue";
import FormBindings from "./components/FormBindings.vue";
import SimpleComponents from "./components/SimpleComponents.vue";
</script>

<!--เรียกใช้ Component ใน template-->
<template>
  <div>
    <SimpleComponents />
    <br /><br />
    
    <FormBindings />
    <br />
    <ConditionsAndLoops />
    <br />
    <br />
    <AttributeBindings />
    <HandingUserInput />
    <CalComponents />
    <HelloWorldExsample />
  </div>
</template>

<style scoped></style>
