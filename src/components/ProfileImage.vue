<script setup>

defineProps({
    image:{
      type: String,
      default: "https://i.imgur.com/9yw1Fyw.jpg",
    }
})

</script>

<template>
    <img :src="image"  class="profile" alt="profile">
</template>
