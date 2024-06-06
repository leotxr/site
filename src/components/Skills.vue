<script setup>
import { ref } from "vue";
const items = ref([
  { icon: "../assets/icons/php-logo.svg", skill: "PHP", level: "Advanced", value: 5 },
  { icon: "", skill: "Laravel", level: "Advanced", value: 5 },
  { icon: "", skill: "Javascript", level: "Intermediate", value: 4 },
  { icon: "", skill: "Vue", level: "Basic", value: 2 },
  { icon: "", skill: "SQL", level: "Intermediate", value: 4 },

]);

</script>
<template>
  <h1>Skills</h1>
  <ul class="max-w-md divide-y divide-gray-200 dark:divide-gray-700">
    <li class="pb-3 sm:pb-4" v-for="(item, index) in items" :key="index">
      <div class="flex items-center space-x-4 rtl:space-x-reverse">
        <div class="flex-shrink-0">
           
        </div>
        <div class="flex-1 min-w-0">
          <p class="text-sm font-medium text-gray-900 truncate dark:text-white">
            {{ item.skill }}
          </p>
          <p class="text-sm text-gray-500 truncate dark:text-gray-400">
            {{ item.level }}
          </p>
        </div>
        <div
          class="inline-flex items-center w-24 space-x-1 text-base font-semibold text-gray-900 dark:text-white"
        >
            <li class="bg-[#b4d3b2] h-3.5 w-3.5 rounded-full" v-for="n in item.value"></li>
        </div>
      </div>
    </li>
  </ul>
</template>
<style scoped>
</style>