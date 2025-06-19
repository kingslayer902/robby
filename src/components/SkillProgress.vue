<template>
  <div>
    <div class="flex justify-between mb-1">
      <span class="text-gray-700 font-medium">{{ label }}</span>
      <span class="text-gray-500">{{ percent }}%</span>
    </div>
    <div class="w-full bg-gray-200 rounded-full h-3">
      <div
        class="bg-blue-600 h-3 rounded-full transition-all duration-700"
        :style="{ width: percent + '%' }"
      ></div>
    </div>
  </div>
</template>

<script setup>
defineProps({
  label: String,
  percent: Number
})
</script>
