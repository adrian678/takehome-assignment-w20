<template>
  <!-- PART 4: Add your code here -->
  <div>
    <h4>{{name}}</h4>
    <Counter
     v-bind:initial_count="this.episodes_seen"
    />

  </div>
</template>

<script>
// PART 4: Add your code here
import Counter from "./Counter";
export default {
  components: {
    Counter
  },
  props: {
    id: Number,
    name: String,
    episodes_seen: Number
  }
};
</script>

<style>
</style>
