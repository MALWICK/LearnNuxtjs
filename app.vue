<template>
  <Home__Welcome />
  <Component :is="Counter" />
</template>

<script setup>
const Counter = resolveComponent("Counter")
</script>