<template>
<div id="app">
    <ActiveUser msg="Hi"/>
    </div>
</template>
<script>
import ActiveUser from './components/ActiveUser.vue'

 export default{
     name:'App',
     
     components:{
         
          ActiveUser
     }
 }
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>