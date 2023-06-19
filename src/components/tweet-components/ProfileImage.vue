<script setup>
defineProps({
  image: {
    type: String,
    default:
      "https://cdn.pixabay.com/photo/2016/02/19/15/46/labrador-retriever-1210559_1280.jpg",
  },
  imageAlt: {
    type: String,
    default: "Alt Image",
  },
});
</script>

<template>
  <img :src="image" class="profile" :alt="imageAlt" />
</template>

<style scoped></style>
