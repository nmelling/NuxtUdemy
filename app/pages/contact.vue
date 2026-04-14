<template>
    <h1>Contact</h1>
    <!-- Possibilité de changer des layouts de manière réactive avec cette méthode auto importée-->
    <button @click="setPageLayout('default')">Change layout</button>
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

// Pour choisir un layout particulier pour cette page
definePageMeta({
  layout: 'secondary',
})
</script>
