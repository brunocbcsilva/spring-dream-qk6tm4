<script setup>
import { ref } from "vue";

const dates = ref([new Date(2024,0), new Date(2024, 3)]);
</script>

<template>
  <img src="./assets/primevue-logo.png" alt="PrimeVue Logo" />
  <h2>PrimeVue Issue Template</h2>
  <p>
    Please create a test case and attach the link of the codesandbox to your
    github issue report.
  </p>
  <Calendar
    v-model="dates"
    selection-mode="range"
    date-format="mm/yy"
    view="month"
    :manual-input="false"
  />
</template>