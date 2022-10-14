<template>
    <div class="tweet">
        <img :image="user.image" class="profile" alt="profile" />
        
        
        <div class="body">
            <div class="top">
                <span class="user">
                    <span class="name">{{props.name}}</span>
                    <span class="handle">{{props.handle}}</span>
                </span>

                <span class="timestamp">{{props.timestamp}}</span>
            </div>

            <p class="message">
                {{props.message}}
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
const props = defineProps({
    name: String,
    img: String,
    handle: String,
    timestamp: String,
    message: String
})

</script>
  
<style scoped>
a {
    color: #42b983;
}
</style>