<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <Child user="Roy Ali Hasan" />
  </div>
</template>

<script>
import Child from "./components/Child.vue";
export default {
  name: "App",
  components: { Child },
};
</script>