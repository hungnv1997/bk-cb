<script setup lang="ts">
import { ref } from "vue";

defineProps<{ msg: string }>();

const count = ref(0);
</script>

<template>
  <main class='c-app'>
  <aside class='c-sidepanel'>
    <nav class='c-sidepanel__nav'>
      <ul>
        <li class='c-sidepanel__nav__li'><a class='c-sidepanel__nav__link' href='' title=''><i data-feather="inbox"></i>Inbox <span class='c-notification c-notification--nav'>404</span></a></li>
        <li class='c-sidepanel__nav__li'><a class='c-sidepanel__nav__link' href='' title=''><i data-feather="edit"></i>Drafts</a></li>
        <li class='c-sidepanel__nav__li'><a class='c-sidepanel__nav__link' href='' title=''><i data-feather="send"></i>Sent</a></li>
        <li class='c-sidepanel__nav__li'><a class='c-sidepanel__nav__link' href='' title=''><i data-feather="star"></i>Favourites</a></li>
        <li class='c-sidepanel__nav__li'><a class='c-sidepanel__nav__link' href='' title=''><i data-feather="trash"></i>Trash</a></li>
      </ul>
    </nav>

    <nav class='c-sidepanel__nav c-sidepanel__nav--spacer'>
      <ul>
        <li class='c-sidepanel__nav__li'><a class='c-sidepanel__nav__link c-sidepanel__nav__link--success' href='' title=''><i data-feather="check-circle"></i>Paid</a></li>
        <li class='c-sidepanel__nav__li'><a class='c-sidepanel__nav__link c-sidepanel__nav__link--pending' href='' title=''><i data-feather="clock"></i>Pending</a></li>
        <li class='c-sidepanel__nav__li'><a class='c-sidepanel__nav__link c-sidepanel__nav__link--warning' href='' title=''><i data-feather="trash"></i>Denied</a></li>
      </ul>
    </nav>

    <nav class='c-sidepanel__nav c-sidepanel__nav--spacer c-friends'>
      <div class='c-sidepanel__header'>
        <h2>Friends<span></span></h2>
        <button>See All</button>
      </div>
    </nav>
  </aside>
  <section class='c-chats'>
    <div class='c-chats__header'>
      <div>
        <label aria-label='Search your active chats.'><i data-feather='search'></i></label>
        <input type='text' placeholder='Search'>
      </div>
    </div>
  </section>
  <section class='c-openchat'>
    <div class='c-openchat__header'>
      <ul>
        <li class='c-openchat__li'><a class='c-openchat__link' href='' title=''>Discover</a></li>
        <li class='c-openchat__li'><a class='c-openchat__link' href='' title=''>Friends</a></li>
        <li class='c-openchat__li'><a class='c-openchat__link c-openchat__link--active' href='' title=''>Messages</a></li>
        <li class='c-openchat__li'><a class='c-openchat__link' href='' title=''>Notifications <span class='c-notification'>2</span></a></li>
        <li class='c-openchat__li'><a class='c-openchat__link' href='' title=''>Help</a></li>
        <li class='c-openchat__li'><img src='https://s.cdpn.io/profiles/user/739421/80.jpg?1557442808' alt=''></li>
      </ul>
    </div>
    <div class='c-openchat__box'>
      <div class='c-openchat__box__header'>
        <img class='c-openchat__box__pp' src='' alt=''>
        <p class='c-openchat__box__name'>Aaron McGuire</p>
        <span class='c-openchat__box__status'></span>
      </div>
      <div class='c-openchat__box__info'></div>
    </div>
  </section>
</main>
</template>

<style scoped lang="css">
</style>
