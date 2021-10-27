<template>
  <div>
    <h1>{{ productName }}</h1>
  </div>
</template>

<script>
export default {
  name: "Parent",
  props: {
    productName: {
      type: Number,
      default: () => {},
    },
  },
};
</script>

<style lang="scss" scoped>
</style>