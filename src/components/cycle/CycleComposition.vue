<template>
<div></div>
</template>

<script lang="ts" setup>
    import { onMounted, onUpdated } from 'vue';
        
    onMounted(() => {
        console.info('Mounted')
    });

    onUpdated(() => {
        console.info('OnUpdated');
    })

</script>

<style scoped>
</style>