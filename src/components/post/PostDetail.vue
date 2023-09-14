<template>
    <div class="post">
        <h3>{{ props.title }}</h3>
        <p>{{ props.content }}</p>
        <input type="text" v-model="message">
        <button @click="handleClick">Saluda</button>
    </div>
</template>

<script lang="ts">
    import { defineComponent, ref, type Ref } from 'vue';

    export default defineComponent({
        name: 'PostDetail',
        props: {
            title: {
                type: String,
                required: true
            },
            content: {
                type: String,
                required: false,
                default: 'Este post no tiene contenido'
            }
        },
        emits: ['sayHi'], // emits para comunicacion vertical ascendente
        setup(props, {emit}) {
            const handleClick = () => {
                emit('sayHi', message.value)
            }
            let message: Ref<string> = ref('');
            return { props, message, handleClick }
        }
    })
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