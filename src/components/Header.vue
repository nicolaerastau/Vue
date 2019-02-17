<template>
  <header>
    <h1>{{title}}</h1>
 <h3 v-onclick:="home">Home</h3>
    <router-link to="/">Home</router-link>
    <router-view></router-view>
  </header>
</template>

<script>
export default {

  data() {
    return {
      title:'App',
      subtitle:'Home'
    }
  }
}
</script>

<style scoped>
header{
  background:#05c46b;
  padding:10px;
}
h1{
  color:#222;
  text-align:center;
}
h2{
  color:#222;
  text-align: center;
}
</style>
