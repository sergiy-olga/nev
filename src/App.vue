<template>
<div class="content tech-steck">
  <div class="icon">
    <v-image :src="htmlImage"></v-image>
    <v-image :src="cssImage"></v-image>
    <v-image :src="jsImage"></v-image>
    <v-image :src="reactImage"></v-image>
    <v-image :src="vectorImage"></v-image>
    <v-image :src="bootstrapImage"></v-image>
  </div>
  <div class="icon">
    <v-image :src="tailwindImage"></v-image>
    <v-image :src="sassImage"></v-image>
    <v-image :src="gitImage"></v-image>
    <v-image :src="greensockImage"></v-image>
    <v-image :src="vscodeImage"></v-image>
    <v-image :src="githubImage"></v-image>
  </div>
  </div>
</template>

<script>
import vImage from "./components/v-image.vue";
import htmlImage from "./assets/html.png";
import cssImage from "./assets/css.png";
import jsImage from "./assets/js.png";
import reactImage from "./assets/react.png";
import vectorImage from "./assets/Vector.png";
import bootstrapImage from "./assets/bootstrap.png";
import tailwindImage from "./assets/tailwind.png";
import sassImage from "./assets/sass.png";
import gitImage from "./assets/git.png";
import greensockImage from "./assets/greensock.png";
import vscodeImage from "./assets/vscode.png";
import githubImage from "./assets/github.png";
export default {
  name: "App",
  components: {
    vImage,
  },
  data() {
       return {
      htmlImage,
      cssImage,
      jsImage,
      reactImage,
      vectorImage,
      bootstrapImage,
      tailwindImage,
      sassImage,
      gitImage,
      greensockImage,
      vscodeImage,
      githubImage,
    };
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
  background: #191919;
}

.icon {
  max-width: 1193px;
  width: 100%;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  background: #191919;
}
.icon:nth-child(1){
padding-bottom: 83px;
}



</style>
