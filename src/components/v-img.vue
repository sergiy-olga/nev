<template>
  <div>
    <img :src="src" :alt="alt" :style="{ width, height }" />
  </div>
</template>

<script>
export default {
  name: "vImage",
  props: {
    width: {
      type: String,
      default: "120px",
    },
    height: {
      type: String,
      default: "120px",
    },
    src: String,
    alt: String,
  },
};
</script>

<style scoped>
</style>