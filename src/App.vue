<script setup>
import { RouterView } from 'vue-router'
import NavBar from './components/NavBar.vue'
import LoginButton from './components/LoginButton.vue'
</script>

<template>
  <div class="container">
    <div class="topBar">
      <img alt="Vue logo" class="logo" src="@/assets/长师校园帮.png" width="125" height="125" />
      <NavBar />
      <LoginButton />
    </div>
    <div class="main">
      <RouterView />
    </div>
  </div>
</template>

<style scoped>
.container {
  display: grid;
  height: 100vh;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  grid-template-rows: 12fr 1fr 1fr 86fr;
  gap: 0px 0px;
  grid-auto-flow: row;
  grid-template-areas:
    'topBar topBar topBar topBar'
    'main main main main'
    'main main main main'
    'main main main main';
}

.topBar {
  background-color: white;
  grid-area: topBar;
  display: flex;
  align-items: center;
  padding: 0 32px;
  max-height: 12vh;
  border-bottom: 3px solid #aaa;
}

.main {
  grid-area: main;
  max-height: 88vh;
}

@media (min-width: 1024px) {
  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
