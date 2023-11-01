<script setup>
  import { watch, ref } from 'vue'
  import HelloWorld from '@/components/HelloWorld.vue'

  const display = (name) => {
    console.log('App vue :' + name)
  }
</script>

<template>
  <HelloWorld
  @update-name="name => display(name)"
  />
</template>

<style>
  .text-red {
    color: red;
  }
  .text-green {
    color: green;
  }
</style>
