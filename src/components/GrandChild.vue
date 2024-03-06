<template>
    <h1>Value {{value}} </h1>
</template>

<script setup>
import {  inject } from 'vue';

const value = inject('value', 'default value')

</script>