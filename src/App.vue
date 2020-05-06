<template>
  <div id="app">
    <Header theTitle="Vue to Due"/>
    <TaskList theTitle="My Task" v-bind:taskList='task'/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import TaskList from "./components/TaskList.vue";

export default {
  name: 'App',
  components: {
    Header,
    TaskList
  },
  data(){
    return{
      task:[
        {id:1, titel:"Learn HTML & CSS", completed:false},
        {id:2, titel:"Learn Javascript", completed:true},
        {id:3, titel:"Learn a JS Framework", completed:false}
      ]
    }
  }
}
</script>

<style>
*{
  margin:0;
  padding: 0;
}
</style>
