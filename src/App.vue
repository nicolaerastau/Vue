<template>
  <div >
    <!-- <div :style="{ 'background-image': 'url (' + backgroundImage +')' }"></div> -->
    <app-header></app-header>
    <app-ninjas></app-ninjas>
    <app-footer></app-footer>
    <app-home></app-home>
    <!-- <router-link to="/">Home</router-link> -->


  </div>
</template>

<script>
import Header from'./components/Header.vue';
import Footer from'./components/Footer.vue';
import Ninjas from'./components/Ninjas.vue';
import Home from'./views/Home.vue';

export default {
   components:{
     'app-header':Header,
     'app-footer':Footer,
     'app-ninjas':Ninjas,
     'app-home':Home,
       // 'backgroundImage':"https://i.imgur.com/jJHygeI.jpg",
   },
  data(){
    return{

    }
  }

}
</script>

<style scoped>
/* background-image:url("https://i.imgur.com/jJHygeI.jpg"); */
</style>
