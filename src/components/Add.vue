<template>
    <div>
   <input type="text" v-model="todo" placeholder="Add Todo">
   <button @click="addTodo">Add</button>
   </div>
</template>

<script>
export default {
     methods:{ 
         addTodo(){
      if(this.todo.length===0){
        return;
      }
      this.todos.push({
        id:Math.random(),
        text:this.todo
      });
    }
   
  }
}
</script>