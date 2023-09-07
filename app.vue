<template>
  <a @click="view('home')">Home</a>
  <a @click="view('counter')">Counter</a>

    <HomeWelcome v-if="page === 'home'" />
 

  <counter v-if="page === 'counter' " />
</template>

<script setup>
const page = ref("home")
function view(name) {
page.value = name
}
</script>