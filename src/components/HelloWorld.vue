<template>
  <div class="hello">
    <h1>{{ counter }}</h1>
    <p>
      <button @click="decrement">Dec</button>
      <button @click="increment">Inc</button>
    </p>
  </div>
</template>

<script>
import { ref } from "vue";
export default {
  setup() {
    const counter = ref(0);

    function increment() {
      counter.value++;
    }

    function decrement() {
      if (counter.value > 0) counter.value--;
    }

    return { counter, increment, decrement };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
button {
  margin: 0 5px;
}
</style>
