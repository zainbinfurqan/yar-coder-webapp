<template>
  <div class="p-2 m-2 border w-auto inline-block text-left">
    <div>
      <i class="p-2 fab fa-medium text-xl" />
    </div>
    <p>Title all the way</p>
    <p>Discription all over the world we have</p>
  </div>
</template>

<script>
export default {
  props: ["service"],
  mounted() {
    console.log(this.service);
  },
};
</script>

<style></style>
