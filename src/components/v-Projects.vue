<template>
  <div class="projects">
    <img :src="src" :style="{ width, height }" />
    <div class="projects_content">
      <h4>{{ msgH4 }}</h4>
      <p>{{ msgText }}</p>
      <p class="small">{{ msgP }}</p>
      <div class="content">
        <div class="top">
          <img :src="src1" :style="{ width1, height1 }" />
          <a href="href">{{ msg }}</a>
        </div>
        <div class="top">
          <img :src="src2" :style="{ width1, height1 }" />
          <a href="href">{{ msg1 }}</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "vProjects",
  props: {
    width: {
      type: String,
      default: "375px",
    },
     width1: {
      type: String,
      default: "20px",
    },
    height: {
      type: String,
      default: "260px",
    },
    height1: {
      type: String,
      default: "20px",
    },
    src: String,
    msgH4: String,
    msgText: String,
    msgP: String,
    href: String,
    msg: String,
    msg1: String,
    src1: String,
    src2: String
  },
};
</script>

<style scoped>
.projects {
  width: 375px;
  height: 567px;
  background: #363636;
  box-shadow: 2px 2px 100px rgba(0, 0, 0, 0.2);
  border-radius: 20px;
  margin-bottom: 65px;
}
h4 {
  font-family: "Poppins";
  font-style: normal;
  font-weight: 500;
  font-size: 28px;
  line-height: 26px;
  text-align: center;
  color: #cccccc;
}
p {
  font-family: "Poppins";
  font-style: normal;
  font-weight: 300;
  font-size: 18px;
  line-height: 26px;
  color: #cccccc;
  text-align: justify;
}
.projects_content {
  width: 314px;
  margin: 0 auto;
}
.small {
  font-family: "Poppins";
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 26px;
  color: #cccccc;
}
.content{
  display: flex;
  justify-content: space-between;
  margin-top: 0%;
}
.top{
  display: flex;
  align-items: center;
}
.top a{
  font-family: 'Poppins';
font-style: normal;
font-weight: 400;
font-size: 16px;
line-height: 26px;
text-decoration-line: underline;
color: #FFFFFF;
margin-left: 12px;
}
</style>