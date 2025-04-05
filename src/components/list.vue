<script setup>
import { ref } from 'vue';
import tusk from './tusk.vue';
defineProps(['tusks'])
const newTusk= ref({
    id:0,
    name:'',
    completed:false
})
function saveTusk(){

}
</script>
<template>
     <!-- Form to Add Task -->
     <div class="flex justify-center mt-16">
        <div class="bg-white p-6 rounded-lg shadow-md mb-8 w-full max-w-3/5">
            <form>
             <div class="mb-4">
                 <label for="task" class="block text-lg font-medium text-gray-700">New Task</label>
                <input type="text" id="task" name="task"
                 class="mt-2 p-2 w-full border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500"
               placeholder="Enter your task here" required />
            </div>
            <button type="submit"
            class="bg-blue-500 text-white p-2 rounded-lg hover:bg-blue-600 w-full">Add Task</button>
    </form>
    <tusk v-for="tusk in tusks" :key="tusk.id" :tusk="tusk"/>
  </div>
</div>

    <!-- Form to Add Task end-->
 
</template>
