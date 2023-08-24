<template>
  <div id="item">

<ul>
<li v-for="task in lista" :key="task.key">
    <spam>{{task.text}}</spam>
    <button @click="deleteItem (task.key)">Concluir</button>
</li>


</ul>

  </div>



 


</template>

<script>
//import Task from './Components/Task.vue'


  export default{
    name: 'item',
    props:[
        'lista',
        'delete'

    ],
    methods:{
        deleteItem(key){
          this.delete(key);
        }
    }
  }
  
</script>

<style scoped>

#item{
    white-space: pre-wrap;
    word-wrap: break-word;
}

ul{
    list-style:none;
    padding: 0px;
    margin-top:20px ;
}
ul li{
    padding: 15px 0;
    display:flex ;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
}

li:not(:first-child){
    border-top:1px solid #eee;
}

a{
    color: aqua;

}

button{
    cursor:pointer;
    background: #ddd;
    color: black;
    border: 0;
    padding: 8px 8px;
    outline: none;
    border-radius :4px;


}

</style>