<template>
  <img alt="Vue logo" src="./assets/logo.png">
 <div class="todo">Todo Lists</div>
 <Delete />
 
</template>

<script>

import Delete from './components/Delete.vue'

export default {
  name: 'App',
  components: {
    Delete,
    
  },
  
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
