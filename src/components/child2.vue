<template>
  <div>
    <button @click="updateTitle">Update Parent title</button>
  </div>
</template>

<script>
export default {
  name: "child2",
  methods: {
    updateTitle() {
        // custom event
      this.$emit("changeTitle", "Parent updated");
    },
  },
};
</script>

<style lang="scss" scoped>
</style>