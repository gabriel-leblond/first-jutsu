<script setup>
  import { computed, ref } from 'vue'
  import HelloWorld from '@/components/HelloWorld.vue'

  const name = ref('Sushi');
  const age = ref(34);
  // Création d'une sentence, c'est une valeur calculer
  // de cette maniere si age ou name change la sentence
  // est actualisé. On utlisie computed.
  const sentence = computed(() => {
    return `Bonjour je suis ${name.value} et j'ai ${age.value}`;
  });

</script>

<template>
  <HelloWorld/>
  <span>{{ sentence }}</span>
</template>

<style>
  .text-red {
    color: red;
  }
  .text-green {
    color: green;
  }
</style>
