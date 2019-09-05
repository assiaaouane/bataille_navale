<template>
  <div id="app">

    <img alt="logo" src="./assets/logo2.png">
<!--    <HelloWorld msg="Welcome to Your Vue.js App"/>-->

    <div class="container" >
      <plateau > </plateau>
    </div>

   <div class = "sidebar"  >
     <Bateaux></Bateaux>
   </div>

  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Plateau from "./components/Plateau";
import Bateaux from "./components/Bateaux";

export default {
  name: 'app',
  components: {
    // HelloWorld ,
    Plateau,
    Bateaux
  }

}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #607386;
  margin-top: 60px;
}

  /*.container{*/

  /*  display: flex;*/
  /*    flex-grow: 1;*/

  /*}*/
  /*  .sidebar{*/

  /*      flex-grow: 1;*/
  /*  }*/
</style>
