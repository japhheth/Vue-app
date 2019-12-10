
 <template>
    <div class="component">
        <h3>You may edit the User here</h3>
        <p>Edit me!</p>
        <P>Hello - {{ name }}</P>
        <button @click="resetName" class="btn btn-primary">reset button</button>
    </div>
   
 </template>
 
 <script>

 export default {

   props: {
       name : {
           type : String,
           required : true
       }
   },
   methods :{
       resetName(){
           this.name = "Japheth";
           this.$emit("nameWasReset", this.name)
       }

   }
 }
 </script>
 
 <style scoped>
    div {
        background-color: lightcoral;
    }
 
 </style>