<template>
  <div class="content">
      <a href="href" >{{msg}}</a>
      <a href="href">{{msg1}}</a>
    </div>

</template>

<script>
export default {
  name: "vFooterTel",
  props: {
    msg: String,
    msg1: String,
  },
};
</script>

<style scoped>
.content{
  width: 355px;
  display: flex;
  justify-content: space-between;
  margin-right: 48px;
}
a{
  text-decoration: none;
  font-family: 'DM Sans';
font-style: normal;
font-weight: 400;
font-size: 18px;
line-height: 26px;
color: #A7A7A7;
}

</style>