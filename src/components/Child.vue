<template>
  <div>
    <h1>Hello from Child</h1>

    <span v-for="product in products" :key="product.id">
      Pc ={{ product.productName }}
      <br />
      Ram:{{ product.Ram }}
      <br />
      Hard:{{ product.Hard }}
      <hr />
    </span>

    <!-- = -->
    {{ user }}
  </div>
</template>

<script>
export default {
  name: "Child",
  props: ["products"],
  methods: {},
};
</script>

