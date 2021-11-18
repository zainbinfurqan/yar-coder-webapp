<template>
  <div>
    <div class="rounded-full flex items-center justify-center">
      <img
        class="rounded-full items-center"
        src="https://picsum.photos/100/100"
        alt="https://picsum.photos/200/300"
      />
    </div>
    <div class="items-center justify-center">
      <h3>Zain Ahmed (Software Engineer)</h3>
      <div class="flex items-center justify-center">
        <i class="p-2 fab fa-facebook-square text-xl" />
        <i class="p-2 fab fa-twitter-square text-xl" />
        <i class="p-2 fab fa-instagram text-xl" />
        <i class="p-2 fab fa-medium text-xl" />
        <i class="p-2 fab fa-dev text-xl" />
        <i class="p-2 fab fa-youtube-square text-xl" />
      </div>
    </div>
    <div class="flex">
      <div v-for="(service, index) of services" v-bind:key="index + 1">
        <ServicesProvide />
      </div>
    </div>
  </div>
</template>

<script>
import ServicesProvide from "./components/providing-services";
export default {
  data() {
    return {
      services: [
        { id: "", title: "Mentorship" },
        { id: "", title: "Colaberation" },
        { id: "", title: "" },
        { id: "", title: "" },
      ],
    };
  },
  component: {
    ServicesProvide,
  },
};
</script>

<style></style>
