<template>
  <div class="component main-page">
       <h1>The User Component</h1>
        <p>I'm an awesome User!</p>
        <button @click="changeName" class="btn btn-primary">Change my name </button>
        <hr>
      <div class="row">
        <div class="col-sm-6">
           <app-user :name="name"></app-user>
        </div>
        <div class="col-sm-6">
           <app-detail :name="name"></app-detail>
        </div>
      </div> 
  </div>
</template>

<script>

  import User from './User.vue'
  import UserDetail from './UserDetail.vue'

export default {
  data : function (){
    return {
      name: "Japheth"
    }
  },
  methods : {
    changeName(){
        this.name = "OJ"
    }
  },
  components : {
    appUser : User,
    appDetail : UserDetail

  }
}
</script>

<style scoped>
    .main-page{
      background-color: lightblue;
    }
</style>

