<template>
  HEADER
  <main class="c-app">
    <!-- <side-bar /> -->
    <search-bar />
    <section class="c-openchat">
      <!-- <nav-bar /> -->
      <chat-space />
      <conversation />
    </section>
  </main>
</template>
<script lang="ts">
import ChatSpace from "../components/common/ChatSpace.vue";
import Conversation from "../components/common/Conversation.vue";
import NavBar from "../components/common/NavBar.vue";
import SearchBar from "../components/common/SearchBar.vue";
import SideBar from "../components/common/SideBar.vue";
export default {
  name: "HomePage",
  components: { SideBar, SearchBar, ChatSpace, NavBar, Conversation },
  setup() {
    return {};
  },
};
</script>

<style scoped lang="css"></style>
