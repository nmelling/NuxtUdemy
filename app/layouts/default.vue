<script setup lang="ts">

// Your script logic here
</script>

<template>
  <div class="container">
      <header>
          <h1>Header</h1>
          <!-- LINKS -->
          <nav>
              <ul>
                  <li>
                      <NuxtLink to="/">Home</NuxtLink>
                  </li>
                  <li>
                      <NuxtLink
                        to="/contact"
                        target="_blank"
                    >Contact</NuxtLink>
                  </li>
              </ul>
          </nav>
      </header>
      <hr />
      <slot />
  </div>
</template>
