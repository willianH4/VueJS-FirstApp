<template>
    <div class="container">
        <PostDetailVue v-for="(post, index) in info" :key="index" title="post.title" content="post.content"/>
    </div>
</template>

<script lang="ts" setup>
import PostDetailVue from './PostDetail.vue';
import type { IPost } from '@/data/interfaces/Post';


    let info:Array<IPost> = [
        {
            title: 'Post 1',
            content: 'Texto del post 1'
        }, 
        {
            title: 'Post 2',
            content: 'Texto del post 2'
        }, 
        {
            title: 'Post 3',
            content: 'Texto del post 3'
        }, 
        {
            title: 'Post 4',
            content: 'Texto del post 4'
        },
        {
            title: 'Post 5',
            content: 'Texto del post 5'
        }
    ]
</script>

<style scoped>
    .container {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
    }

</style>