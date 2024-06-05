<script setup>
defineProps({
  label: {
    type: String,
    required: true
  },
  link: {
    type: String,
    required: false
  }
})
</script>
<template>
    <a type="button" class="ring-black ring-1 bg-[#b4d3b2] text-black mr-2">{{label}}</a>
</template>
<style scoped>

</style>