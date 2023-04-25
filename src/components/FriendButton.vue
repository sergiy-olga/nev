<template>
  <div>
    <button v-on:click="onClick">{{ msg }}</button>
    <button v-on:click="onClick">{{ msg }}</button>
  </div>
</template>

<script>
export default {
  name: "FriendButton",
  props: {
    msg: Object,
  },
  methods: {
    onClick() {
      alert("саша");
    },
  },
};
</script>

<style scoped>
h1 {
  text-shadow: 2px 2px green;
}
</style>
