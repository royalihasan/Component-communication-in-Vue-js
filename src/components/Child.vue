<template>
  <div>
  
<!--  -->
   <b> {{ user }} </b>
    <span v-for="product in products" :key="product.id">
      Pc ={{ product.productName }}
      <br />
      Ram:{{ product.Ram }}
      <br />
      Hard:{{ product.Hard }}
      <hr />
    </span>
<!-- button -->
  <div>
    
 </div>
  </div>
</template>

<script>
export default {
  name: "Child",
  props: ["products","user"],
  methods: {},
};
</script>

