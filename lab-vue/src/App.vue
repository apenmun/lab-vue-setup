<template>
  <div>
<Micomponente/>
  </div>
  <h2: class ="counter > 0 ? 'positive':'negative'"> {{ counter }}</h2:>
  <button @click="increment"> Increment </button>
  <button @click="decrement"> Decrement</button>
  <button @click="reset" Reset> Reset </button>
</template>

<script setup>
import Micomponente from "../src/components/Micomponente.Vue.vue";
import {ref} from "vue";

const counter = ref (0);
const increment = () => counter.value++;
const decrement = () => counter.value--;
const reset = () => (counter.value = 0);
</script>

<style lang="scss" scoped>

</style>
