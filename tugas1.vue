<template>
  <div id="app">
    <h1>Numbers 1 to 50</h1>
    <ul>
      <li v-for="number in numbers" :key="number">{{ number }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      numbers: Array.from({ length: 50 }, (v, k) => k + 1)
    };
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  margin-top: 60px;
}
</style>
