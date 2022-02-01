<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <h1>Vue3 template</h1>
  <ul class="list">
    <li v-for="dependency in dependencies" :key="dependency">
      {{ dependency }}
    </li>
  </ul>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "App",
  data() {
    return {
      dependencies: ["📝 Typescript", "💅 Prettier", "✏️ Eslint"] as string[],
    };
  },
});
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.list {
  font-size: 1.5em;
  margin: 0;
  padding: 0;
  list-style: none;
}
</style>
