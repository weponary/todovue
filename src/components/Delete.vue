<template>
    <div v-for="todo in todos" v-bind:key="todo.id">
   {{todo.text}}
   <button @click="removeTodo(todo.id)">Delete</button>
 </div>
 <Add/>
</template>
<script>
import Add from './Add.vue'
export default {
    components:{
        Add
    },
    data(){
    return{
      todo:'',
      todos:[
        {
        id:Math.random(),
        text:'Soshal',
      },
       {
        id:Math.random(),
        text:'Dahal',
      },
      ]
    }
  },
     methods:{
    removeTodo(todoId){
      this.todos= this.todos.filter(todo => todo.id !== todoId);
    },
     }
}
</script>