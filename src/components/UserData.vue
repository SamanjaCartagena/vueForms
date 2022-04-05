<template>
<section>
    <form @submit.prevent="submitData">
    <input type="text" placeholder="Your name" v-model="enteredName"/>
    <input type="text" placeholder="Your profession" v-model="enteredWork"/>
    <button>Set User Data</button>
    </form>
</section>
</template>
<script>

export default{
    emits:['set-data'],
    data(){
        return{
            enteredName:'',
            enteredWork:''
        }
    }, methods:{
        submitData(){
            this.$emit('set-data', this.enteredName, this.enteredWork);
            this.enteredName='';
            this.enteredWork='';
        }
    }
  
}
</script>
