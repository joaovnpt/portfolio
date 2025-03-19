<script setup>
import NavBar from './components/NavBar.vue';

</script>

<template>
  <NavBar class="navbar" />
  <RouterView />
</template>

<style scoped>
.navbar {
  margin: 2rem;
}
</style>
