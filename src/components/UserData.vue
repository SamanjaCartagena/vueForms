<template>
<div>
<form>
  <input  type="email" placeholder="Email"/>
  <input type="password" placeholder="password"/>
  <button @click="submit">Submit</button>
</form>
</div>

</template>
<script>
import ActiveUser from './ActiveUser.vue';

export default{
    name:'UserData',
    components:{
        ActiveUser, 
        
    }
}
</script>
