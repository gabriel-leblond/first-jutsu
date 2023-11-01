<script setup>
  import { ref } from 'vue'
  // import d'un component enfant
  import HelloWorld from '@/components/HelloWorld.vue'

  const user = ref({
    name: 'sushi',
    age: 10,
  });

  const display = () => {
    console.log(user.value)
  }

</script>

<template>
  <HelloWorld>
    <p>{{ user.name }}</p>
  </HelloWorld>
  <div v-if="user.age > 15">
    Vous êtes majeur !
  </div>
  <div v-else>
    Vous êtes n'êtes pas majeur !
  </div>

</template>

<style>

</style>
