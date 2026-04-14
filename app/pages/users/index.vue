<template>
    <h1>Users</h1>
</template>

<script setup lang="ts">
const route = useRoute();

// Ne définit pas les headers html d'une page mais permet d'ajouter des propriétés à la route
// Ne peut pas utiliser de propriétés réactives
  definePageMeta({
    title: 'Users',
    meta: [
      { name: 'description', content: 'Users description...' },
    ],
    something: 'Hey...'
  })

// Contient les infos définie au sein de definePageMeta
console.log(route.meta);
</script>
