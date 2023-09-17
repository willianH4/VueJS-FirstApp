<template>
    <div class="post">
        <h3>{{ props.title }}</h3>
        <p>{{ props.content }}</p>
        <input type="text" v-model="message">
        <button @click="handleClick">Saluda</button>
    </div>
</template>

<script lang="ts" setup>
    import { defineProps, defineEmits, ref, type Ref } from 'vue';

    const props = defineProps({
        title: String, 
        content: String
    });

    const emit = defineEmits(['sayHi']);

    const handleClick = () => {
        emit('sayHi', message.value)
    }
    let message: Ref<string> = ref('');

</script>

<style scoped>
    .post {
        width: 300px;
        border-radius: 10px;
        height: auto;
        min-height: 100px;
        background-color: antiquewhite;
        text-align: center;
        margin: 10px;
        padding: 10px;
    }

</style>