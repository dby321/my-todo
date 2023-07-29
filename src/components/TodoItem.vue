<template>
  <li>
    <input type="checkbox" v-model="todo.done">
    <span class="todoText"> {{todo.todoText  }}</span>
  </li>
</template>
<script> 
export default {
  name: 'TodoItem',
  data(){
    return {

    }
  },
  props:['todo']
  
}
</script>
<style scoped>
li{
  list-style: none;
}
.todoText{
  background-color: skyblue;
  display:inline-block;
  height: 20px;
  width: 100%;
}
</style>