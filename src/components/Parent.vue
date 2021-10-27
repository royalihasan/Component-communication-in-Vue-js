<template>
  <div>
    <h1>{{ productName }}</h1>
      <button @click="hit">Click Me</button>
  </div>
</template>

<script>
export default {
  name: "Parent",
   methods: {
        hit() {
           console.log("clicked")
        }
    },
    //!
  props: {
    productName: {
      type: String,
      default: () => {},
    },
   
  },
};
</script>

<style lang="scss" scoped>
</style>