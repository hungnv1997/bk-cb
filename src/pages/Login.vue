<script lang="ts">
import ChatSpace from "../components/common/ChatSpace.vue";
import NavBar from "../components/common/NavBar.vue";
import SearchBar from "../components/common/SearchBar.vue";
import SideBar from "../components/common/SideBar.vue";
export default {
  components: { SideBar, SearchBar, ChatSpace, NavBar },
  setup() {
    return {};
  },
};
</script>

<template>
  <main class="c-app">
    <side-bar />
    <search-bar />
    <section class="c-openchat">
      <nav-bar />
      <chat-space />
    </section>
  </main>
</template>

<style scoped lang="css"></style>
