<template>
    <span class="timestamp">{{props.timestamp}}</span>
</template>
<script setup>
const props = defineProps ({
        name: String, 
        image: String, 
        handle: String,
        timestamp: String,
        message: String
})
</script>
<style scoped>
</style>