
 <template>
    <div class="component">
        <h3>You may edit the User here</h3>
        <p>Edit me!</p>
        <P>Hello - {{ name }}</P>
    </div>
   
 </template>
 
 <script>

 export default {
   props: ['name']
 
 }
 </script>
 
 <style scoped>
    div {
        background-color: lightcoral;
    }
 
 </style>