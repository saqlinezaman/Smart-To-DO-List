<script setup>
import { ref } from 'vue';
import list from './components/list.vue';
const ToDoList = ref([
    // {id:0,name:'Input your tusk',completed:false},
])
</script>

<template>
<div class="">
  <list :tusks="ToDoList"/>
</div>

</template>

<style scoped>

</style>
