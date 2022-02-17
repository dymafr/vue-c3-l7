<template>
  <h1 @click="userClick">Bonjour tout le monde !</h1>
  <input @input="userInput" type="text" />
</template>

<script setup lang="ts">
function userClick(event: MouseEvent) {
  console.log(event);
}

function userInput(event: Event) {
  const target = event.target as HTMLInputElement;
  target.value = 'Bonjour';
  console.log(event);
}
</script>

<style></style>
