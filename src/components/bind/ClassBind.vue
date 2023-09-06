<template>
    <p v-bind:class="{'danger' : hasError}">El mensaje se ha enviado correctamente.</p>
</template>

<script lang="ts" setup>
    let hasError = true;
</script>

<style scoped>
    .danger {
        color: red;
    }

</style>