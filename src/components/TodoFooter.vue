<template>
  <div>
    <input type="checkbox" :checked="allChecked">
   完成任务数{{todoDoneCount}}/总任务数{{ todoList.length }}
  </div>
</template>
<script> 
export default {
  name: 'TodoFooter',
  data(){
    return {

    }
  },
  computed:{
    todoDoneCount(){
      return this.todoList.filter(value=>value.done==true).length;
    },
    allChecked(){
      return this.todoDoneCount==this.todoList.length;
    }
  },
  props:["todoList"]

}
</script>
<style lang="less" scoped>

</style>