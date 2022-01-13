<template>
  <div class="flex flex-col px-16 m-2">
    <div
      v-for="(blog, index) of blogs"
      v-bind:key="index + 1"
      class="
        border
        rounded
        p-2
        max-w-2xl
        m-2
        min-w-5xl
        bg-gray-100
        cursor-pointer
        drop-shadow-2xl
        hover:bg-gray-200 drop-shadow-2xl
      "
      v-bind:class="[index % 2 === 0 ? 'self-start' : 'self-end']"
    >
      <div class="flex flex-row max-w-2xl min-w-5xl">
        <div>
          <img src="https://picsum.photos/200/220" />
        </div>
        <div class="px-2 text-left">
          <p class="text-xl font-semibold">{{ blog.title }}</p>
          <p>{{ blog.details }}</p>
          <div class="">
            <div class="flex">
              <p class="font-medium">Publish Date:</p>
              <span>{{ formatDate(blog.createdAt) }}</span>
            </div>
            <p class="font-medium cursor-pointer">Read full article</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// import Articals from "../Blogs/components/articals";
import moment from "moment";
import { data } from "../../data/data";
export default {
  data() {
    return {
      blogs: data.blogs,
    };
  },
  components: {
    // Articals,
  },
  methods: {
    formatDate: function (date) {
      return moment(date).format("DD/MM/YYYY");
    },
    isEven: function (value) {
      if (value % 2 == 0) return true;
      else return false;
    },
  },
};
</script>

<style></style>
