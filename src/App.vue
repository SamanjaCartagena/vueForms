<template>
<div>
   <active-user :username="user.name" :userwork="user.work"></active-user>
   <user-data @set-data="setUserData"></user-data>

    </div>
</template>
<script>
import ActiveUser from './components/ActiveUser.vue'
import UserData from './components/UserData.vue'

 export default{
   data(){
       return{
           user:{
               name:'Samanja',
               work:'Programmer'
           }
       }
   }, 
   components:{
       ActiveUser,
       UserData
   },
   methods:{
       setUserData(name,work){
          this.user={
              name:name,
              work:work
          }
       }
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