<template>
<h1>Cars page</h1>
<p>{{ $route.params.name[0] }}</p>
</template>

<script setup lang="ts">
// Ce spread au sein du nom de la route permet de capturer n'importe quel chemin dans l'url, meme si la page n'existe pas dans l'arborescence Nuxt
// Ex: /cars/red/big -> redirige sur cette page
// Cette écriture s'appelle une 'catch-all route'
// $route.params.name -> Array de params

const route = useRoute();
console.log(route.params.name);
console.log(Array.isArray(route.params.name)) // true
</script>
