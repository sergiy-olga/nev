<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="Welcome to Your Vue.js App" />
  <FirstButton msg="кнопка" />
  <FriendButton msg="кнопка 2" />
  <VImageHtml src_html="./assets/html.png" />
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import FirstButton from "./components/FirstButton.vue";
import FriendButton from "./components/FriendButton.vue";
import VImageHtml from "./components/v-imageHtml.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    FirstButton,
    FriendButton,
    VImageHtml,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
