<template>
  <div>
    <h2>{{titleH2}}</h2>
    <h3>{{titleH3}}</h3>
  </div>
</template>

<script>
export default {
  name: "vTitleH2H3",
  props: {
    titleH2: String,
    titleH3: String,
  },
};
</script>

<style scoped>
h2 {
  font-family: 'Poppins';
font-style: normal;
font-weight: 700;
font-size: 48px;
line-height: 26px;
text-align: center;
color: #CCCCCC;
}
h3 {
  font-family: 'Poppins';
font-style: normal;
font-weight: 400;
font-size: 32px;
line-height: 26px;
text-align: center;
color: #A7A7A7;
}
div {
  margin-bottom: 147px;
}
</style>