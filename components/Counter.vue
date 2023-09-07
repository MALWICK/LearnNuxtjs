<template>
  <template>
    <div>
      <div>Hello World</div>
      <div>
        <button @click="increment">Increment</button>
        <p>{{ count }}</p>
        <button @click="decrement">Decrement</button>
      </div>
    </div>
  </template>
</template>

<script setup>
const count = ref(0);

function increment() {
  count.value++;
}

function decrement() {
  count.value--;
}
</script>
</template>