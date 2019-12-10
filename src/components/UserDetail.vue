<template>
    <div class="component">
        <h3>You may view the User Details here</h3>
        <p>Many Details</p>
        <p> Hello - {{ name }}</p>
        <button @click="resetToOld" class="btn btn-primary"> Reset button </button>
       
    </div>
       
</template>

<script>
export default {
    props : {
        name : {
         type:   String,
        required : true
        } 
    },
    methods : {
        resetToOld(){
            this.name = "Changed"
        }
    }
  

}
</script>

<style scoped>
       div {
        background-color: lightgreen;
    }
   

</style>