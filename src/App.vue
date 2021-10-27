<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <Parent />
    <!-- = -->
    <Child v-bind:products="products" />
    <!-- = -->
    <child2 v-on:changeTitle="updateTitle($event)" />
    <h1>{{ title }}</h1>
  </div>
</template>

<script>
import Child from "./components/Child.vue";
import Child2 from "./components/child2.vue";

import Parent from "./components/Parent.vue";

export default {
  name: "App",
  components: { Child, Parent, Child2 },
  data() {
    return {
      title: "Vie js",
      products: [
        { productName: "Hp compaq 6005", Ram: "4GB", Hard: "240GB" },
        { productName: "Dell", Ram: "2GB", Hard: "40GB" },
        { productName: "Acer", Ram: "6GB", Hard: "140GB(ssd)" },
        { productName: "Mac", Ram: "12GB", Hard: "1TB" },
      ],
    };
  },
  methods: {
    updateTitle(title) {
      this.title = title;
    },
  },
};
</script>