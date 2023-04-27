<template>
  <div>
    <img :src="src_html" alt="html logo" :width="120" :height="100" />
  </div>
</template>

<script>
export default {
  name: "VImageHtml",
  props: {
    width: String,
    heigth: String,
    src_html: String,
  },
};
</script>

<style scoped>
</style>