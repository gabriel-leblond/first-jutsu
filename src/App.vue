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
    <template v-slot:name>
      <p>{{ user.name }}</p>
    </template>
    <template v-slot:age>
      <p>{{ user.age }}</p>
    </template>
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
