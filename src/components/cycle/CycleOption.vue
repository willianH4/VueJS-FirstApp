<template>
<div></div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

    export default defineComponent({
        name: 'CycleOption',
        created() {
            // actions when created component
            console.info('Created');
        },
        mounted() {
            // actions when mounted
            console.log('Mounted');
        },
        updated() {
          // actions when after create 
          console.info('Updated');
        },
        unmounted() {
            // actions when destroy component
            console.log('Unmounted')
        },
    })
</script>

<style scoped>
</style>