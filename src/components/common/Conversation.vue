<template>
  <div
    class="c-openchat__box__info"
    v-bind="containerProps"
    style="height: 100vh"
  >
    <!-- <ul>
      <li class="c-bubble">
        <img class="c-bubble__image" src="" alt="" />
        <p class="c-bubble__msg">
          I want you to design something for me<span class="c-bubble__timestamp"
            >2020-08-20 15:30:00</span
          >
        </p>
      </li>
      <li class="c-bubble my-message">
        <img class="c-bubble__image" src="" alt="" />
        <p class="c-bubble__msg">
          Cool, what did you have in mind?<span class="c-bubble__timestamp"
            >2020-08-20 15:32:00</span
          >
        </p>
      </li>
      <li class="c-bubble">
        <img class="c-bubble__image" src="" alt="" />
        <p class="c-bubble__msg">
          I need a new website for my shop<span class="c-bubble__timestamp"
            >2020-08-20 15:50:00</span
          >
        </p>
      </li>
      <li class="c-bubble my-message">
        <img class="c-bubble__image" src="" alt="" />
        <p class="c-bubble__msg">
          Cool, how much have you got for a budget?<span
            class="c-bubble__timestamp"
            >2020-08-20 17:30:00</span
          >
        </p>
      </li>
      <li class="c-bubble">
        <img class="c-bubble__image" src="" alt="" />
        <p class="c-bubble__msg">
          I will pay you in exposure mate!aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
          aaaaaaaaaaaaaa aaaaaaaaaaaaaaaaaaaaaaaaa<span
            class="c-bubble__timestamp"
            >2020-08-20 18:21:00</span
          >
        </p>
      </li>
    </ul> -->
    <!-- <div class="list">
      <div v-for="(item, index) in virtualList" :key="index">
        {{ item.name }}
      </div>
    </div> -->
    <ul v-bind="wrapperProps">
      <li
        class="c-bubble"
        v-for="(item, index) in list"
        :key="item.id"
        :class="index % 2 ? 'my-message' : ''"
      >
        <img class="c-bubble__image" src="" alt="" />
        <p class="c-bubble__msg">
          I want you to design something for me<span class="c-bubble__timestamp"
            >2020-08-20 15:30:00</span
          >
        </p>
      </li>
    </ul>
  </div>
</template>

<script>
import { ref } from "vue";
import { useVirtualList } from "@vueuse/core";
export default {
  name: "Conversation",
  setup() {
    const data = ref([
      { id: 1, name: "Item 1" },
      { id: 2, name: "Item 2" },
      { id: 3, name: "Item 3" },
      { id: 4, name: "Item 4" },
      { id: 5, name: "Item 5" },
      { id: 6, name: "Item 6" },
      { id: 7, name: "Item 7" },
      { id: 8, name: "Item 8" },
      { id: 9, name: "Item 9" },
      { id: 10, name: "Item 10" },
      { id: 11, name: "Item 11" },
      { id: 12, name: "Item 12" },
      { id: 13, name: "Item 13" },
      { id: 14, name: "Item 14" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
      { id: 15, name: "Item 15" },
    ]);

    // Số lượng item hiển thị trên màn hình
    const itemHeight = 80;
    const itemsPerRow = 12;
    const visibleCount = 12;

    // Sử dụng `useVirtualList` để tạo danh sách ảo
    const { containerProps, wrapperProps, list } = useVirtualList(data, {
      itemHeight,
      itemsPerRow,
      visibleCount,
    });

    return {
      containerProps,
      wrapperProps,
      list,
    };
  },
};
</script>

<style lang="scss" scoped></style>
