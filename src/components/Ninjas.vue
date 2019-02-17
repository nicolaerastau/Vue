<template>
 <div id="ninjas">
   <ul>
     <li v-for="ninja in ninjas" v-on:click="ninja.show = !ninja.show">
       <h2>{{ninja.name}}</h2>
       <h3 v-show="ninja.show">{{ninja.speciality}}</h3>
     </li>
   </ul>
 </div>
</template>

<script>

export default {
  data() {
    return {
       ninjas:[
         {name:'Nicolae',speciality:'Frontend developer', show:false},
         {name:'Staff',speciality:'Backend developer', show:false},
         {name:'Staff',speciality:'UX designer', show:false},
         {name:'Staff',speciality:'Vue Components', show:false},
         {name:'Staff',speciality:'Web Security', show:false},
         {name:'Staff',speciality:'Vue Components', show:false}
       ]
    }
  }
}
</script>

<style scoped>
  #ninjas{
    width: 100%;
    max-width:500px;
    margin:40px auto;
    padding:0 20px;
    box-sizing:border-box;

  }
  ul{
    display:flex;
    /* flex-direction: column; */
    /* flex-wrap:wrap; */
    flex-direction:column;
    list-style-type:none;
    padding: 0;
  }
  li{
    flex-grow: 1;
    flex-basis: 200px;
    height:200px;
    text-align:center;
    padding:30px;
    border:1px solid #222;
    margin:10px;
    background-color:#16a085;

  }
  h3{
    font-size:30px;
    color: #080707;

  }
  h2{
    font-size:40px;
    color:#0a0a0a;
  }
  h2:hover{
      text-decoration: underline;
  font-size:40px;
  color:#c0392b;
  text-shadow: 0.7px 0.7px #f8f9f5;
  -webkit-transition-property: all;
  transition-property: all;
  -webkit-transition-duration: 0.5s;
  transition-duration: 0.5s;
  }
</style>
