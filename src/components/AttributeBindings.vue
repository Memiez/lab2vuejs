<script setup lang="ts"></script>

<template>
  <p>
    <span title="message">
      Hover your mouse over me for a few seconds to see my dynamically bound
      title!
    </span>
  </p>

  <p class="red">
    <span>This should be red... but click me to toggle it.</span>
  </p>

  <p style="color: green">
    <span>
      This should be green, and should toggle between green and blue on click.
    </span>
  </p>
</template>

<style scoped></style>
