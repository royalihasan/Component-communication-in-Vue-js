<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <Parent productName="Products Details" />
    <!-- = -->
    <Child v-bind:products="products" />
  </div>
</template>

<script>
import Child from "./components/Child.vue";
import Parent from "./components/Parent.vue";

export default {
  name: "App",
  components: { Child,Parent },
  data() {
    return {
      products: [
        { productName: "Hp compaq 6005", Ram: "4GB", Hard: "240GB" },
        { productName: "Dell", Ram: "2GB", Hard: "40GB" },
        { productName: "Acer", Ram: "6GB", Hard: "140GB(ssd)" },
        { productName: "Mac", Ram: "12GB", Hard: "1TB" },
      ],
    };
  },
};
</script>