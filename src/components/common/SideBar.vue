<template>
  <aside class="c-sidepanel">
    <nav class="c-sidepanel__nav">
      <ul>
        <li class="c-sidepanel__nav__li">
          <a class="c-sidepanel__nav__link" href="" title=""
            ><i data-feather="inbox"></i>Inbox
            <span class="c-notification c-notification--nav">404</span></a
          >
        </li>
        <li class="c-sidepanel__nav__li">
          <a class="c-sidepanel__nav__link" href="" title=""
            ><i data-feather="edit"></i>Drafts</a
          >
        </li>
        <li class="c-sidepanel__nav__li">
          <a class="c-sidepanel__nav__link" href="" title=""
            ><i data-feather="send"></i>Sent</a
          >
        </li>
        <li class="c-sidepanel__nav__li">
          <a class="c-sidepanel__nav__link" href="" title=""
            ><i data-feather="star"></i>Favourites</a
          >
        </li>
        <li class="c-sidepanel__nav__li">
          <a class="c-sidepanel__nav__link" href="" title=""
            ><i data-feather="trash"></i>Trash</a
          >
        </li>
      </ul>
    </nav>

    <nav class="c-sidepanel__nav c-sidepanel__nav--spacer">
      <ul>
        <li class="c-sidepanel__nav__li">
          <a
            class="c-sidepanel__nav__link c-sidepanel__nav__link--success"
            href=""
            title=""
            ><i data-feather="check-circle"></i>Paid</a
          >
        </li>
        <li class="c-sidepanel__nav__li">
          <a
            class="c-sidepanel__nav__link c-sidepanel__nav__link--pending"
            href=""
            title=""
            ><i data-feather="clock"></i>Pending</a
          >
        </li>
        <li class="c-sidepanel__nav__li">
          <a
            class="c-sidepanel__nav__link c-sidepanel__nav__link--warning"
            href=""
            title=""
            ><i data-feather="trash"></i>Denied</a
          >
        </li>
      </ul>
    </nav>

    <nav class="c-sidepanel__nav c-sidepanel__nav--spacer c-friends">
      <div class="c-sidepanel__header">
        <h2>Friends<span></span></h2>
        <button>See All</button>
      </div>
    </nav>
  </aside>
</template>

<script>
export default {
  name: "SideBar",
  setup() {
    return {};
  },
};
</script>

<style lang="scss" scoped></style>
