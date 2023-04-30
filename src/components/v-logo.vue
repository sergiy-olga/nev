<template>
  <div>
    <img :src="src" alt="logo" :style="{ width, height }" />
  </div>
</template>

<script>
export default {
  name: "vLogo",
  props: {
    width: {
      type: String,
      default: "97px",
    },
    height: {
      type: String,
      default: "59px",
    },
    src: String,
  },
};
</script>

<style scoped>
</style>