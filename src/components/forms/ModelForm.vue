<template>
    <form>
        <input type="text" v-model="inputText">
        <input type="checkbox" name="check" v-model="agree"> Acepto terminos y condiciones
        <select v-model="country">
            <option value="Spain">Spain</option>
            <option value="Mexico">Mexico</option>
            <option value="El Salvador">El Salvador</option>
        </select>
    </form>
    <h3>{{ inputText }}</h3>
</template>

<script lang="ts" setup>
    import { ref } from 'vue';

    let inputText = ref('')
    let agree = ref(true)
    let country = ref('El Salvador')
</script>

<style scoped>
</style>