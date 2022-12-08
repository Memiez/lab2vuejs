<script setup lang="ts">
export interface Eatable {
  id: number;
  text: string;
}
import type { PropType } from "vue";
const prop = defineProps({
  todo: {
    type: Object as PropType<{ id: number; text: string }>,
    required: true,
  },
});
</script>

<template>
  <li>{{ todo.text }}</li>
</template>
