<template>
    <ul>
        <li v-for="(country, index) in countries" :key="index">{{ country }}</li>
    </ul>
</template>

<script lang="ts" setup>
    import { ref, type Ref } from 'vue';
    
    let countries:Ref<Array<string>> = ref([
        'Spain', 'France', 'UK', 'Italy', 'Portugal'
    ])
</script>

<style scoped>
</style>