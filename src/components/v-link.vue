<template>
    <div>
           <a :href="href">{{ msg }}</a> 
          </div>
</template>

<script>
export default {
  name: "vLink",
  props: {
    href: String,
    msg: String
  },
};
</script>

<style scoped>
a {
  text-decoration: none;
  font-family: 'DM Sans';
font-style: normal;
font-weight: 500;
font-size: 20px;
line-height: 26px;
color: #A7A7A7;
}
</style>