<template>
  <div class="text">
    <p :style="{color, fontStyle, fontWeight, fontSize, lineHeight}">{{ msg }}</p>
  </div>
</template>

<script>
export default {
  name: "vFooterText",
  props: {
    msg: String,
        color: {
      type: String,
      default: "#CCCCCC",
    },
    fontStyle:{
       type: String,
      default: "normal", 
    },
    fontWeight: {
      type: String,
      default: "700",
    },
    fontSize: {
      type: String,
      default: "18px",
    },
    lineHeight: {
      type: String,
      default: "26px",
    },
  },
};
</script>

<style scoped>

</style>