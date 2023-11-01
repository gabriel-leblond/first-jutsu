<script setup>
  import { ref } from 'vue'
  // import d'un component enfant
  import HelloWorld from '@/components/HelloWorld.vue'

  const user = ref({
    name: 'sushi',
    age: 33,
  });

  // const display = () => {
  //   console.log(name.value);
  // };
</script>

<template>
  <HelloWorld :user ="user"/>
  <input type="text" v-model="user.name" />
  <input type="text" v-model="user.age" />
</template>

<style>

</style>
