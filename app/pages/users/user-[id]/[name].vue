<template>
<h1>User by id and Name</h1>
<p>ID: {{ $route.params.id }}</p>
<p>NAME: {{ $route.params.name }}</p>
</template>

<script setup lang="ts">
const route = useRoute();
console.log('id: ', route.params.id);
</script>
