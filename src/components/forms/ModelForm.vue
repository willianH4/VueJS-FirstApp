<template>
    <form>
        <input type="text" v-model="inputText">
    </form>
    <h3>{{ inputText }}</h3>
</template>

<script lang="ts" setup>
    import { type Ref, ref } from 'vue';

    let inputText:Ref<string> = ref('');
</script>

<style scoped>
</style>