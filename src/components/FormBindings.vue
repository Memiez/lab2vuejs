<script setup lang="ts">
import { ref } from "vue";
const text = ref("Edit Me");
const checked = ref(true);
const checkedNames = ref(["Memo"]);
const picked = ref("One");
</script>

<template>
  <h2>Text Input</h2>
  <input v-model="text" /> {{ text }}

  <h2>Checkbox</h2>
  <input type="checkbox" v-model="checked" ide="checkbox" />
  <label for="checkbox"> Checked: {{ checked }}</label>

  <h2>Multiple Checkbox</h2>
  <input type="checkbox" v-model="checkedNames" id="Memo" value="Memo" />
  <label for="Memo">Memo </label>
  <input type="checkbox" v-model="checkedNames" id="P.Kob" value="P.Kob" />
  <label for="P.Kob">P.Kob</label>
  <input type="checkbox" v-model="checkedNames" id="์Nadej" value="Nadej" />
  <label for="Nadej">Nadej</label>
  <p>Checked names</p>
  <pre> {{ checkedNames }} </pre>

  <h2>Radio</h2>
  <input type="radio" id="one" value="One" v-model="picked" />
  <label for="one">One </label>
  <input type="radio" id="two" value="Two" v-model="picked" />
  <label for="two">Two </label> <br />
  <span>Picked {{ picked }}</span>
</template>
