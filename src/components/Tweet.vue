<script setup>
import ProfileImage from './ProfileImage.vue';
import User from './User.vue';
import Timestamp from './Timestamp.vue';
import Message from './Message.vue';
import Actions from './Actions.vue';

  defineProps({
    name:{
      type: String,
    },
    handle:{
      type: String,
    },
    timestamp:{
      type: String,
    },
    message:{
      type: String,
    },
    image:{
      type: String,
      default: "https://i.imgur.com/9yw1Fyw.jpg",
    },
  }
  )
</script>

<template>
  <div class="tweet">

    <ProfileImage :image="image"/>

    <div class="body">
      <div class="top">
        <span class="user">
          <User :name="name" :handle="handle"/>
        </span>
        <Timestamp :timestamp="timestamp"/>

      </div>

      <Message :message="message"/>

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
