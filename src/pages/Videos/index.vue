<template>
  <div>
    <div class="flex flex-row m-2 overflow-x-auto">
      <div
        v-for="(video, index) of videos"
        v-bind:key="index + 1"
        class="
          video-content-card
          border
          rounded
          p-2
          max-w-2xl
          m-2
          min-w-5xl
          bg-gray-100
          cursor-pointer
          drop-shadow-2xl
          hover:bg-gray-200 hover:h-72
          drop-shadow-2xl
        "
      >
        <div class="flex flex-col max-w-2xl min-w-5xl">
          <div>
            <img src="https://picsum.photos/200/220" />
          </div>
          <div class="px-2 text-left">
            <p class="text-xl font-semibold">{{ video.title }}</p>
            <p>{{ video.description }}</p>
            <div class="">
              <div class="flex">
                <p class="font-medium">Publish Date:</p>
                <span>{{ formatDate(video.createdAt) }}</span>
              </div>
              <p class="font-medium cursor-pointer">Read full article</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import moment from "moment";
import { data } from "../../data/data";

export default {
  data() {
    return {
      videos: data.contentVideos,
    };
  },
  components: {
    // Articals,
  },
  methods: {
    formatDate: function (date) {
      return moment(date).format("DD/MM/YYYY");
    },
  },
};
</script>

<style>
.video-content-card {
  transition: 0.3s;
}
.video-content-card:hover {
  margin: 30px;
}
</style>
