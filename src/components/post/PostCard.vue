<template>
    <div class="post-card">
        <h3>Titulo</h3>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Aperiam velit, harum dolore consequuntur deserunt similique, quae quos placeat recusandae, in ullam ratione quasi deleniti ex minima molestiae nisi possimus? Ut!</p>
        <PostButton />
    </div>
</template>

<script lang="ts" setup>
    import PostButton from './PostButton.vue';
</script>

<style scoped>
    .post-card {
        border-radius: 15px;
        padding: 10px;
        margin: 5px;
        border: 1px solid #ccc;
    }
</style>