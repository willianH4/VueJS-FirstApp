<template>
<div>
    <label for="sub">SubTotal</label>
    <input type="number" v-model="subTotal">
    <h3>Total a pagar: {{ totalVat }} ({{ vat }}%)</h3>
</div>
</template>

<script lang="ts" setup>
import {type Ref, ref, computed} from 'vue';
    
    const vat = 21;
    let subTotal:Ref<number> = ref(0);
    const totalVat = computed(() => (vat * subTotal.value) / 100 )

</script>

<style scoped>
</style>