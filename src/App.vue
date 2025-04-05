<script setup>
import { ref } from 'vue';
import list from './components/list.vue';
const ToDoList = ref([
    {id:1,name:'tusk 1',completed:false},
    {id:2,name:'tusk 2',completed:false},
    {id:3,name:'tusk 3',completed:false},
    {id:4,name:'tusk 4',completed:false},
    {id:5,name:'tusk 5',completed:false},
])
</script>

<template>

<p>{{ ToDoList }}</p>
<div class="">
  <list :tusks="ToDoList"/>
</div>

</template>

<style scoped>

</style>
