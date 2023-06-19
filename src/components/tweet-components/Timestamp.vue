<script setup>
defineProps({
  timestamp: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <span class="name">{{ timestamp }}</span>
</template>

<style scoped></style>
