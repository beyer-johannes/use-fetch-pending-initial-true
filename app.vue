<script setup>
const { pending, execute } = useFetch(
  "https://api.chucknorris.io/jokes/random",
  {
    immediate: false,
  }
);
</script>

<template>
  <div>
    <div>Pending is: {{ pending }}</div>

    <button @click="execute">Submit</button>
  </div>
</template>
