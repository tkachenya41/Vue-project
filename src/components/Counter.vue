<template>
  <div class="counter">
    <h3>Counter {{ count }}</h3>
    <button @click="increase">Increase</button>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
  name: "Counter",
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    increase() {
      this.count += 1;
    },
  },
});
</script>

<style>
.counter {
  display: flex;
  flex-direction: row;
  gap: 1rem;
}
</style>
