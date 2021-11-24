<template>
  <div class="flex flex-wrap items-center justify-center">
    <div v-for="(artical, index) of articals" v-bind:key="index + 1">
      <Articals />
    </div>
  </div>
</template>

<script>
import Articals from "../Blogs/components/articals";
export default {
  data() {
    return {
      articals: [{ id: "1" }, { id: "2" }, { id: "3" }, { id: "4" }],
    };
  },
  components: {
    Articals,
  },
};
</script>

<style></style>
