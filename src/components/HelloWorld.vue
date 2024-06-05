<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div class="space-y-2 text-left">
    <h1 class="text-4xl font-bold">{{ msg }}</h1>
    <span class=""></span>
    <h3 class="text-xl font-regular">
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. 
      Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. 
    </h3>
  </div>
</template>
