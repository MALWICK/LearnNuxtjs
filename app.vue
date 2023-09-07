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

<script>
import { ref } from 'vue';

export default {
  setup() {
    const count = ref(0);

    function increment() {
      count.value++;
    }

    function decrement() {
      count.value--;
    }

    return {
      count,
      increment,
      decrement
    };
  },
};
</script>