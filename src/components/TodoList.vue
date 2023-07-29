<template>
 <ul class="todoItem">
  <TodoItem v-for="todo in todoList" :key="todo.id" :todo="todo"></TodoItem>
 </ul>
</template>
<script>
import TodoItem from "@/components/TodoItem.vue" 
export default {
  name: 'TodoList',
  data(){
    return {

    }
  },
  components:{
    TodoItem
  },
  props:['todoList']
  
}
</script>
<style lang="less" scoped>

</style>