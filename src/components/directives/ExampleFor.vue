<template>
    <ul>
        <li v-for="(country, index) in countries" :key="index">{{ country.name }}</li>
    </ul>
</template>

<script lang="ts" setup>
    import type { ICountry } from '@/data/interfaces/Country';
    import { ref, type Ref } from 'vue';
    
    let countries:Ref<Array<ICountry>> = ref([
        {
            code: 'es',
            name: 'Spain'
        },
        {
            code: 'en',
            name: 'England'
        },
        {
            code: 'sv',
            name: 'El Salvador'
        }
    ])
</script>

<style scoped>
</style>