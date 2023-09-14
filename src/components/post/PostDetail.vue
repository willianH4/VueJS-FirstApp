<template>
    <div class="post">
        <h3>{{ props.title }}</h3>
        <p>{{ props.content }}</p>
    </div>
</template>

<script lang="ts">
    import { defineComponent } from 'vue';

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
        setup(props) {
            return { props }
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