<template>
    <span class="user">
        <span class="name">{{props.name}}</span>
        <span class="handle">{{props.handle}}</span>
    </span>
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