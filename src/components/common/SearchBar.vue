<template>
  <section class="c-chats">
    <div class="c-chats__header">
      <div>
        <label aria-label="Search your active chats."
          ><i data-feather="search"></i
        ></label>
        <input type="text" placeholder="Search" />
      </div>
    </div>
  </section>
</template>

<script lang="ts">
export default {
  name: "SearchBar",
};
</script>

<style lang="scss" scoped></style>
