<script setup>
// j'importe la variable subTittle depuis le parrent App.vue
// une variable qui communique du Parent vers Enfant est une props
const props = defineProps(['user']);

</script>

<template>
  <h1> Hello Wolrd</h1>
  <p>Bonjour je m'apelle {{ props.user.name }} et j'ai {{ props.user.age }} ans</p>
</template>

<style>

</style>
