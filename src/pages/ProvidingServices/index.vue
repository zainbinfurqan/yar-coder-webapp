<template>
  <div class="flex flex-wrap items-center justify-center">
    <div v-for="(service, index) of services" v-bind:key="index + 1">
      <div class="p-2 m-2 border w-auto inline-block text-left max-w-sm">
        <div>
          <i class="p-2 text-xl" :class="'fas fa-' + service.icon" />
        </div>
        <p class="font-medium">{{ service.title }}</p>
        <p>{{ service.description }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      services: [
        {
          id: "1",
          title: "Mentorship",
          icon: "map-signs",
          description:
            "I can guid you in your inital career stage and can support you in you road map to software engineer ",
        },
        {
          id: "2",
          title: "Colaberation",
          icon: "hands-helping",
          description:
            "I can collaberate with different industries/sfotware houses for different events",
        },
        {
          id: "3",
          icon: "chalkboard-teacher",
          title: "Meetups/Volunter",
          description: "I can work as volunter/speaker in different Meetups",
        },
      ],
    };
  },
};
</script>

<style></style>
