<script setup>

</script>

<template>

<div class="max-w-4xl mx-auto mt-10">
    <h1 class="text-3xl font-semibold text-center mb-16 bg-blue-500 te text-white ">To-Do List</h1>
    <!-- Form to Add Task -->
    <div class="bg-white p-6 rounded-lg shadow-md mb-12">
      <form>
        <div class="mb-4">
          <label for="task" class="block text-lg font-medium text-gray-700">New Task</label>
          <input type="text" id="task" name="task" class="mt-2 p-2 w-full border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500" placeholder="Enter your task here" required />
        </div>
        <button type="submit" class="bg-blue-500 text-white p-2 rounded-lg hover:bg-blue-600 w-full">Add Task</button>
      </form>
    </div>

    <!-- Task Cards (Flexbox Layout) -->
    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-5 mb-10">
      <!-- Example Task Cards -->
       <!-- card 1  -->
      <div class="bg-white p-6 rounded-lg shadow-md flex flex-col">
        <h3 class="text-xl font-semibold text-gray-700 mb-4">Buy groceries</h3>
        <p class="text-gray-600 mb-4">Complete the grocery shopping for the week.</p>
        <button class="bg-red-500 text-white px-4 py-2 rounded-lg hover:bg-red-600 self-start">Delete</button>
      </div>
      <!-- card 2 -->
      <div class="bg-white p-6 rounded-lg shadow-md flex flex-col">
        <h3 class="text-xl font-semibold text-gray-700 mb-4">Complete homework</h3>
        <p class="text-gray-600 mb-4">Finish the math and science homework assignments.</p>
        <button class="bg-red-500 text-white px-4 py-2 rounded-lg hover:bg-red-600 self-start">Delete</button>
      </div>
    </div>

  </div>

</template>

<style scoped>

</style>
