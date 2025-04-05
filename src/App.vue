<script setup>
import { ref } from 'vue';
import list from './components/list.vue';
const ToDoList = ref([
    // {id:0,name:'Input your tusk',completed:false},
])
</script>

<template>
  <h1 class="  justify-center text-center my-10 text-4xl font-bold  text-neutral-700">Saqline Zaman To Do List </h1>
  <hr class=" mx-116 border-t-3 ">
<div class="">
  <list :tusks="ToDoList"/>
</div>

</template>

<style scoped>

</style>
