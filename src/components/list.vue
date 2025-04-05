<script setup>
import { ref } from 'vue';
import tusk from './tusk.vue';
const props = defineProps(['tusks'])
const add =ref(false)
const newTusk= ref({
    id:0,
    name:'',
    completed:false
})
function saveTusk(){
add.value=false;
newTusk.value.id = props.tusks.length + 1;
props.tusks.push(newTusk.value);
newTusk.value ={
     id:0,
    name:'',
    completed:false
}
}
</script>
<template>
     <!-- Form to Add Task -->
     <div class="flex justify-center mt-16">
        <div class="bg-white p-6 rounded-lg shadow-md mb-8 w-full md:max-w-3/5">
             <div class="mb-4">
                 <label for="task" class="block text-lg font-medium text-gray-700">New Task</label>
                <input type="text" id="task" name="task"
                 class="mt-2 p-2 w-full border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500"
               placeholder="Enter your task here" v-model="newTusk.name" />
            </div>
            <div class="">
                <button @click="saveTusk"
            class="bg-blue-500 text-white p-2 rounded-lg hover:bg-blue-600 w-full">Add Task</button>
            </div>
    <tusk v-show="!tusk.completed" v-for="tusk in tusks" :key="tusk.id" :tusk="tusk"/>
  </div>
</div>

    <!-- Form to Add Task end-->
 
</template>
