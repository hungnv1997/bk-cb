<script setup></script>

<template>
  <div>
    <!-- <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a> -->
    <p>
      <!-- <router-link to="/home">Home</router-link>
      &nbsp;
      <router-link to="/login">Add</router-link> -->
      <component :is="$route.meta.layout || 'div'"></component>
    </p>
  </div>

  <!-- <HelloWorld msg="Vite + Vue" /> -->
</template>

<style scoped></style>
