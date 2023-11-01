<script setup>
  import { watch, ref } from 'vue'
  import HelloWorld from '@/components/HelloWorld.vue'

  const name = ref('Rik');
  const age = ref(34);
  // Watcher > si la variable est modifier
  // J'ai accès a
  // son ancienne valeur et ça nouvelle valeur
  // je vais pouvoir executer du code
  watch(name, (newValue, oldValue) => {
    console.log(newValue, oldValue);
  })

</script>

<template>
  <HelloWorld/>
  <span>{{ sentence }}</span>
  <input v-model="name"/>
  <input v-model="age"/>
</template>

<style>
  .text-red {
    color: red;
  }
  .text-green {
    color: green;
  }
</style>
