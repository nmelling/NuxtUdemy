<template>
    <h1>Contact</h1>
</template>


<script setup lang="ts">
// Toute déclaration au sein du composant permet d'overrider la valeur du parent
// Supporte la réactivité avec l'utilisation suivante:
const title = ref('Contact');

setTimeout(() => {
  title.value = "Contact Réactif";
  console.log(title.value)
}, 2000)

useHead({
  titleTemplate: title,
})
</script>
