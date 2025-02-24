<script setup>
import { ref } from 'vue';

const showText = ref(true);
</script>

<template>
  <button @click="showText = !showText">Umschalten</button>
  <p v-if="showText">Ich bin sichtbar!</p>
  <p v-else>Ich bin versteckt!</p>
</template>
