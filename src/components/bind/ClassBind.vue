<template>
    <p v-bind:style="{ backgroundColor: '#ccc', color: c }">El mensaje se ha enviado correctamente.</p>
    <button @click="handleClick">Cambiar color</button>
</template>

<script lang="ts" setup>
    import { ref } from 'vue';
    
    let c = ref('#FFF');
    const handleClick = () => {
        c.value = '#ff0000'
    }
</script>

<style scoped>
</style>