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
  <HelloWorld :user ="user"/>
  <input type="text" v-model="user.name" @input="display"/>
  <input type="text" v-model="user.age" @input="display"/>
  <div v-if="user.age > 15">
    Vous êtes majeur !
  </div>
  <div v-else>
    Vous êtes n'êtes pas majeur !
  </div>

</template>

<style>

</style>
