<script setup>

defineProps({
    message: {
        type: String,
    },
})

</script>

<template>
    <p class="message">
        {{ message }}
    </p>
</template>
