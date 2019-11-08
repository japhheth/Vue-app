<template>
  <div class="container">
    <div class="row">
      <div class="col-sm-12">
          <hello-world></hello-world>
      </div>
      
    </div>
    
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {

  components: {
     helloWorld : HelloWorld
  }
}
</script>

<style>
   div.component {
        border: 1px solid black;
        padding: 30px;
        
    }

</style>
