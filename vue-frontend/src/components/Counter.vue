<template>
  <div>
    <p>I'm a Counter!</p>
    <h3> Current count: {{count}}</h3>
    <button v-on:click="count++">Increment count!</button>
    <button v-on:click="count--">Decrement count!</button>
  </div>
</template>

<script>
export default {
  props:{
    initial_count: Number
  },
  data: function() {
    return {
      count: this.initial_count
    };
  }
};
</script>

<style>
</style>

