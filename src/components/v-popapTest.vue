<template>
  <div class="popap">
    <div class="popap_button">
      <slot name="popapClose"></slot>
    </div>
    <div class="project-popap">
      <div class="project_image_popap">
        <slot name="popapImg"></slot>
      </div>
      <div class="project_text_content_popap">
        <div class="project_title_popap">
          <slot name="popapTitle"></slot>
        </div>
        <div class="project_text_popap">
          <slot name="popapText1"></slot>
        </div>
        <div class="project_text2_popap">
          <slot name="popapText2"></slot>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "vPopapTest",
  props: {},
};
</script>

<style scoped>
.popap{
  max-width: 1000px;
  width: 100%;
  background: grey;
  margin: 0px auto;
  position: fixed;
  top: 10px;
  left: auto;
  right: auto;
  color: black;
}
.project-popap{
max-width: 900px;
width: 100%;
margin: 0 auto;
margin-top: 20px;
}
.project_image_popap .img img{
  border-radius: 50px;
}
.popap_button{
  text-align: end;
  margin: 10px;
}
</style>