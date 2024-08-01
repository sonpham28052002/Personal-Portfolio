<template>
  <div class="navmenu">
    <a href="#" rel="noopener noreferrer"
      ><img src="../../../assets/logo-portfolio.png" alt="Vue logo" class="logo"
    /></a>
    <nav>
      <font-awesome-icon
        @click="toggleMenu"
        class="toggle-btn"
        :icon="showMenu ? ['fas', 'xmark'] : ['fas', 'bars']"
      />
      <div class="menu">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/project">project</RouterLink>
        <RouterLink to="/contact">contact</RouterLink>
        <RouterLink to="/skill">skill</RouterLink>
      </div>
      <div :class="{ open: showMenu, close: !showMenu }" class="dropdown_menu">
        <RouterLink @click="closeMenu" to="/">Home</RouterLink>
        <RouterLink @click="closeMenu" to="/about">About</RouterLink>
        <RouterLink @click="closeMenu" to="/project">project</RouterLink>
        <RouterLink @click="closeMenu" to="/contact">contact</RouterLink>
        <RouterLink @click="closeMenu" to="/skill">skill</RouterLink>
      </div>
    </nav>
  </div>
</template>
<script setup lang="ts">
import { RouterLink } from 'vue-router'
import { ref } from 'vue'
var showMenu = ref(false)
var toggleMenu = () => {
  showMenu.value = !showMenu.value
}
var closeMenu = () => {
  showMenu.value = false
}
</script>
<style scoped>
@import url('../Navbar/NavbarComponent.css');
@import url('../Navbar/NavbarComponentResponsive.css');
</style>
