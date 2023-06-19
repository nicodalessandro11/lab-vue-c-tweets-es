<script setup>
defineProps({
  userName: {
    type: String,
    required: true,
  },
  userHandle: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <span class="user">
    <span class="name">{{ userName }} </span>
    <span class="handle">{{ userHandle }}</span>
  </span>
</template>

<style scoped></style>
