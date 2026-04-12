<template>
  <div>
    <NuxtPage />
  </div>
</template>

<script setup lang="ts">
// Toute déclaration ici est transmise aux niveaux inférieurs de l'app
// Permet de générer le head de la page HTML
// Deux façons de s'en servir

// useHead({
//   title: 'Awesome app',
//   meta: [
//     { name: 'description', content: 'Some description...' }
//   ],
//   link: [
//     {
//       rel: 'stylesheet',
//       href: 'https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.8/css/bootstrap-grid.min.css',
//     }
//   ]
// })

// SeoMeta n'est pas réactif
// type Protected: Si une propriété n'existe pas, rien n'est appliqué
useSeoMeta({
  title: 'Awesome app',
  ogTitle: 'Awesome app',
  description: 'Some description..',
  ogDescription: 'Some description..'
})

// Le mieux est d'utiliser de base useSeoMeta si pas besoin de réactivité car type protected.
// Et useHead au sein des enfants pour override avec réactivité.
</script>
