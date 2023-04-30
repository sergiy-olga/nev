<template>
  <div>
    <img :src="src" alt="logo" :style="{ width, height }" />
  </div>
</template>

<script>
export default {
  name: "vHeaderIcon",
  props: {
    width: {
      type: String,
      default: "30px",
    },
    height: {
      type: String,
      default: "30px",
    },
    src: String,
  },
};
</script>

<style scoped>

</style>