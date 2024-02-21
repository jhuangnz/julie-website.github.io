<script setup lang="ts">
import { RouterLink } from "vue-router";
</script>

<template>
  <header>
    <H1 class="title">JULIE HUANG</H1>
    <nav>
      <div class="photography">
        <RouterLink to="/">PHOTOGRAPHY</RouterLink>
      </div>
      <div class="about">
        <RouterLink to="/about">ABOUT</RouterLink>
      </div>
    </nav>
  </header>
  <RouterView />
</template>

<style scoped>
  header {
    position: fixed;
    line-height: 1.5;
    max-height: 100vh;
  }

  nav {
    display: flex;
    flex-direction: column;
    width: 100%;
    text-align: left;
    margin-top: 2rem;
  }

  nav a.router-link-exact-active {
    color: grey;
  }

  .title {
    font-size: 4rem;
  }

  .photography {
    font-size: 30px;
    font-weight: 400;
  }

  .about {
    font-size: 30px;
  }
</style>
