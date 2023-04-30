<template>
  <div>
    <img :src="src" alt="html logo" :style="{ width, height }" />
  </div>
</template>

<script>
export default {
  name: "vImageTitle",
  props: {
    width: {
      type: String,
      default: "349px",
    },
    height: {
      type: String,
      default: "349px",
    },
    src: String,
  },
};
</script>

<style scoped>
</style>