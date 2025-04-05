<script setup>
defineProps(['tusk']);
</script>

<template>
     <li class="flex items-center justify-between bg-white px-4 py-3 rounded-lg shadow-md  my-5">
        <p class="font-bold">{{ tusk.id }}</p> <label class="flex items-center w-full pl-4">
        <input type="checkbox" v-model="tusk.completed" class="h-5 w-5 text-blue-500 border-gray-300 rounded mr-3">
    <span :class="tusk.completed ? 'text-gray-400' : 'text-gray-800'" class="text-base font-medium">
      {{ tusk.name }}
    </span>
  </label>
</li>

</template>

<style scoped>

</style>
