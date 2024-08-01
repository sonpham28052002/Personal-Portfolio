<script setup lang="ts">
import RenderNavView from './components/Nav/RenderNavView.vue'
import NavbarComponent from './components/Nav/Navbar/NavbarComponent.vue'
</script>

<template>
  <header>
    <NavbarComponent />
  </header>
  <section><RenderNavView /></section>
</template>
<style scoped>
header {
  height: 8%;
}
section {
  height: 92%;
}
</style>
