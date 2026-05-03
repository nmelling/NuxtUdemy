<template>
    <h1>Home</h1>
    <hr>
    <button @click="router.push('/contact')">
        Go to contacts
    </button>
</template>

<script setup lang="ts">
const router = useRouter();


</script>
