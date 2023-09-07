<template>
    <form>
        <input type="text" v-model="inputText">
    </form>
    <h3>{{ inputText }}</h3>
</template>

<script lang="ts">
    import { defineComponent, ref } from 'vue';

    export default defineComponent({
        setup() {
            let inputText = ref('')
            return { inputText }
        }
    })
</script>

<style scoped>
</style>