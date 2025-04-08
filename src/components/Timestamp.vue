<script setup>

defineProps({
    timestamp:{
      type: String,
    },
})

</script>

<template>
    <span class="timestamp">{{timestamp}}</span>
</template>
