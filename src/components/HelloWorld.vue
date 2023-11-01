<script setup>
import { ref } from "vue";
const emit = defineEmits(['updateName']);

const handleUpdate = (event) => {
  emit("updateName", event.target.value);
}

const name = ref('');

</script>

<template>

<h1>Hello World</h1>
{{ name }}
<input type="text" v-model="name" @input="handleUpdate"/>

</template>

<style>

</style>
