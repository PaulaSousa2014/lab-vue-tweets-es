<template>
  <div class="tweet">
    <ProfileImage :image="user.image" />

    <div class="body">
      <div class="top">
        <User userData="user" :name="props.name" :handle="props.handle"/>
        <Timestamp :timestamp="props.timestamp"/>
      </div>

      <p class="message">
        {{ props.message }}
      </p>

      <div class="actions">
        <!-- Font Awesome icons -->
        <i class="far fa-comment"></i>
        <i class="fas fa-retweet"></i>
        <i class="far fa-heart"></i>
        <i class="fas fa-share"></i>
      </div>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>
<script setup>
import ProfileImage from './ProfileImage.vue'
import User from './/User.vue'
import Timestamp from './Timestamp.vue'

const props = defineProps({
  name: String,
  image: String,
  handle: String,
  timestamp: String,
  message: String,
});
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
