<script setup>
  import { ref } from 'vue'
  import HelloWorld from '@/components/HelloWorld.vue'
  // const subTitle = "Je suis le sous titre du parent"
  // je crée une variable réactive avec ref
  const name = ref("");
  const age = ref("");
</script>

<template>
  <!-- Je passe subTitle en props a l'enfant HelloWorld.vue -->
  <!-- si j'acualise au dessus ma variable elle est maintenant -->
  <!-- lié dynamiquement a l'enfant grâce au v-bind -->
  <HelloWorld :name ="name" :age ="age"/>
  <input type="text" v-model="name" />
  <input type="text" v-model="age" />
</template>

<style>

</style>
