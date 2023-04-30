<template>
  <div class="footer_text">
      <p class="p" :style="color">{{msg}}</p>
    </div>

</template>

<script>
export default {
  name: "vFooterText",
  props: {
    msg: String,
    color:{
      type: String,
    } 
  },
};
</script>

<style scoped>
.p{
 font-family: 'Poppins';
font-style: normal;
font-weight: 400;
font-size: 18px;
line-height: 26px;
text-align: center;
color: #A7A7A7;
background: linear-gradient(90deg, #13B0F5 -2.06%, #E70FAA 100%),
linear-gradient(0deg, #A7A7A7, #A7A7A7);

}
</style>