<template>
    <h1>
        Counter View {{counterStore.counter}}
    </h1>
    <Button @click="counterStore.incrementBy(1)" label="+1" class="p-button-raised p-button-outlined p-button-secondary" />
    <Button @click="counterStore.incrementBy(2)" label="+2" class="p-button-raised p-button-outlined p-button-success" />
    <Button @click="counterStore.incrementBy(5)" label="+5" class="p-button-raised p-button-outlined p-button-help" />

</template>
<script lang="ts" setup>
import {useCounterStore} from '../stores/counter';
import Button from 'primevue/button';
const counterStore = useCounterStore();
</script>