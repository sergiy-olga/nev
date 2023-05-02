<template>
  <div class="v-container">
    <slot></slot>
    <slot name="icon"></slot>
  </div>
</template>

<script>
export default {
  name: "vContainer",
  props: {
  },
};
</script>

<style scoped>
</style>