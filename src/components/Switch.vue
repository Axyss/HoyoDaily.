<script setup lang="ts">
const model = defineModel<boolean>()
</script>

<template>
  <label class="relative inline-flex items-center cursor-pointer">
    <input
      type="checkbox"
      class="sr-only peer"
      v-model="model"
    >
    <div
      class="w-11 h-6 bg-gray-700 peer-focus:outline-none rounded-full
             peer peer-checked:after:translate-x-full peer-checked:after:border-white
             after:content-[''] after:absolute after:top-[2px] after:left-[2px]
             after:bg-white after:border-gray-300 after:border after:rounded-full
             after:h-5 after:w-5 after:transition-all peer-checked:bg-primary"
    ></div>
  </label>
</template>
