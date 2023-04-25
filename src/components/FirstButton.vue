<template>
  <div>
    <h1>мої кнопки</h1>
    <button v-on:click="onClick">{{msg}}</button>
    <button v-on:click="onClick" style="color: red">{{msg}}</button>
  </div>
</template>

<script>
export default {
  name: 'FirstButton',
  props: {
    msg: String
  },
   methods: {
    onClick(){
      alert("привіт");
    }
  }
}
</script>

<style scoped>
button{
  background-color: blue;
  width: 100px;
  color: antiquewhite;
  border-radius: 5px;
  margin: 10px;
}
div{
  border: 2px solid black;
  padding-bottom: 20px;
  background-color: chartreuse;
}
h1{
  text-shadow: 2px 2px green;
}
</style>
