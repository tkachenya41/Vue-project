<template>
  <h1>Vue project</h1>
  <Counter />
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Counter from "./components/Counter.vue";

export default defineComponent({
  name: "App",
  components: {
    Counter,
  },
});
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;

  #app {
    width: 15rem;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    gap: 1rem;
    justify-content: center;
  }
}
</style>
