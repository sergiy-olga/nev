<template>
    <div>
           <a :href="href" :style="{color, textDecoration}">{{ msg }}</a> 
          </div>
</template>

<script>
export default {
  name: "vLinc",
  props: {
    href: String,
    msg: String,
    color: {
type: String,
default: "#A7A7A7"
    },
    textDecoration: {
        type: String,
        default: "none",
    }
  },
};
</script>

<style scoped>

</style>