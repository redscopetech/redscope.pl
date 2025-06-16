<script setup>
import { RouterLink, RouterView } from 'vue-router'
import LoadingScreen from './components/LoadingScreen.vue';
import OkeyCookiesModal from './components/OkeyCookiesModal.vue';
</script>

<template>
  <LoadingScreen></LoadingScreen>
  <OkeyCookiesModal></OkeyCookiesModal>
  <header>
    <img alt="Vue logo" class="logo" src="@/assets/redscope-tech-logo.png" width="125" height="125" />

    <div class="wrapper">

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped></style>
