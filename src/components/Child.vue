<template>
  <div>
    <h1>Hello from Child</h1>
    {{ user }}
  </div>
</template>

<script>
export default {
  name: "Child",
  props: ["user"],
};
</script>

