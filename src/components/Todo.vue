<template>
  <div>
    <TodoHeader />
    <TodoList :todoList="todoList" />
    <TodoFooter :todoList="todoList"/>
  </div>
</template>
<script>
import TodoHeader from "@/components/TodoHeader.vue"
import TodoList from "@/components/TodoList.vue"
import TodoFooter from "@/components/TodoFooter.vue"
export default {
  name: 'Todo',
  data() {
    return {
      todoList: [
        { id: '001', todoText: '喝酒', done: false },
        { id: '002', todoText: '抽烟', done: false },
        { id: '003', todoText: '烫头', done: false }
      ]
    }
  },
  components: {
    TodoHeader, TodoList,TodoFooter
  }
}
</script>
<style lang="less" scoped></style>