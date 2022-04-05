<template>
    <section>
      <h2>{{username}}
          </h2>
          <h3>{{userwork}}</h3>
    </section>
</template>
<script>
export default{
  props:{
      
      username:{
          type:String,
          required:true
      },
      userwork:{
          type:String,
          required:true
      }
  }
   
}

</script>
<style>
section{
    margin:2rem auto;
    max-width:40rem;
    border-radius:12px;
    border:1px solid #ccc;
}
</style>
