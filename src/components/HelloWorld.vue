<script setup>
// j'importe la variable subTittle depuis le parrent App.vue
// une variable qui communique du Parent vers Enfant est une props
const props = defineProps(['name', 'age']);

</script>

<template>
  <h1> Hello Wolrd</h1>
  <p>Bonjour je m'apelle {{ props.name }} et j'ai {{ props.age }} ans</p>
</template>

<style>

</style>
