<template>
<div>
  <slot>
      <p>red</p>
    </slot>
    <p>green</p>
    <slot name="pap">
      <p>color</p>
    </slot>
    <slot name="papa">
      <p>color</p>
    </slot>
    
    </div>
</template>

<script>
export default {
  name: "vPopap",
  props: {
  },
};
</script>

<style scoped>
</style>