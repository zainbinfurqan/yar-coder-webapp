<template>
  <div class="flex flex-wrap items-center justify-center">
    <div v-for="(item, index) of supportList" v-bind:key="index + 1">
      <div class="p-2 m-2 border w-auto inline-block text-left max-w-sm">
        <div>
          <div v-if="item.isImgIcon">
            {{ item.imgIcon }}
          </div>
          <i
            v-if="item.imgIcon.length == 0"
            class="p-2 text-xl"
            :class="item.icon"
          />
        </div>
        <p class="font-medium">{{ item.title }}</p>
        <p>{{ item.description }}</p>
      </div>
    </div>
  </div>
</template>

<script>
import BuyMeACoffee from "../../assets/icons/svgs/buy_me_a_coffee";
export default {
  data() {
    return {
      supportList: [
        {
          id: "1",
          title: "Buy me a coffee",
          description: "",
          icon: "fas fa-hands-helping",
          isImgIcon: false,
          imgIcon: BuyMeACoffee,
        },
        {
          id: "3",
          title: "Plant a seed in your area",
          description: "",
          icon: "fab fa-pagelines",
          isImgIcon: false,
          imgIcon: "",
        },
        {
          id: "2",
          title: "Share my content with other",
          description: "",
          icon: "fas fa-share-alt",
          isImgIcon: false,
          imgIcon: "",
        },
        {
          id: "4",
          title: "Do share the knowledge with other without share my content",
          icon: "fas fa-chalkboard-teacher",
          description: "",
          isImgIcon: false,
          imgIcon: "",
        },
      ],
    };
  },
};
</script>

<style></style>
