<script setup>
  import { ref, provide } from 'vue'

  import ChildComponent from './components/ChildComponent.vue'

  const name = ref('Kaer')
  provide('value', name)

</script>

<template>

  <input type="text" v-model="name">
  <ChildComponent />

</template>
