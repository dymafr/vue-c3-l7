<template>
  <h1 @click="userClick.left.once">Bonjour tout le monde !</h1>
  <form @submit.prevent="formSubmit">
    <button>Envoyer</button>
  </form>
</template>

<script setup lang="ts">
function userClick(event: MouseEvent) {
  console.log(event);
}
function formSubmit() {
  console.log('Envoyé');
}
</script>

<style></style>
