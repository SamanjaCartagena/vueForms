<template>
    <UserData />
    
</template>
<script>
import UserData from './UserData.vue';
export default{
    name:'ActiveUser',
    props:{
       msg:String
    },
    components:{
        UserData
    }
   
}

</script>
<style scoped>
h2{
    color:black
}
</style>
