<template>
  <div id="app">

<header>
  Minhas tarefas
</header>

<Task> </Task>



  </div>



 


</template>

<script>
import Task from './Components/Task.vue'


  export default{
    name: 'App',
    components :{
      Task
       
  

    
  }
  }
  
</script>

<style>

header{

  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 80px;
  font-size: 40px ;
  color: aliceblue;
}


</style>