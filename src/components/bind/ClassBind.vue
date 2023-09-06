<template>
    <p v-bind:style="{ backgroundColor: '#ccc', color: c }">El mensaje se ha enviado correctamente.</p>
    <button @click="handleClick">Cambiar color</button>
</template>

<script lang="ts">
    import { defineComponent } from 'vue';
    export default defineComponent({
        name: 'ClassBind',
        data() {
            return {
                c: '#fff'
            }
        },
        methods: {
            handleClick() {
                this.c = '#ff0000'
            }
        },
    })
</script>

<style scoped>
</style>