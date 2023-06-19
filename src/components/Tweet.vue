<script setup>
import Message from "./tweet-components/Message.vue";
import ProfileImage from "./tweet-components/ProfileImage.vue";
import Timestamp from "./tweet-components/Timestamp.vue";
import User from "./tweet-components/User.vue";
import Actions from "./tweet-components/Actions.vue";

defineProps({
  tweet: {
    type: Object,
    required: true,
  },
  imageChild: {
    type: String,
    required: true,
  },
  imageAltChild: {
    type: String,
    required: true,
  },
  userNameChild: {
    type: String,
    required: true,
  },
  userHandleChild: {
    type: String,
    required: true,
  },
  timestampChild: {
    type: String,
    required: true,
  },
  messageChild: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <div class="tweet">
    <ProfileImage :image="imageChild" :image-alt="imageAltChild" />

    <div class="body">
      <div class="top">
        <User :userName="userNameChild" :userHandle="userHandleChild" />

        <Timestamp :timestamp="timestampChild" />
      </div>

      <Message :message="messageChild" />

      <Actions />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>
