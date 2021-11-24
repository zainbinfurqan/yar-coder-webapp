<template>
  <div class="p-2 flex h-screen">
    <Portal target="#popup-target">
      <div
        class="
          absolute
          p-2
          m-2
          rounded
          bg-green-600
          text-white
          -mt-2
          transform
          trasition-all
          mt-0
        "
      >
        <p>Successfully!</p>
      </div>
    </Portal>
    <div class="w-2/4 bg-local" style="background-color: #00a0c8; height: 100%">
      <img
        style="margin: 0 auto; top: 39%; position: relative"
        class="w-full"
        src="../../assets/images/Contact-Information.jpeg"
        alt="../../assets/images/Contact-Information.jpeg"
      />
    </div>
    <div class="w-2/4 self-center">
      <div class="p-3">
        <input class="w-full h-8 my-2 border rounded px-2" placeholder="Name" />
        <input
          class="w-full h-8 my-2 border rounded px-2"
          placeholder="Email"
        />
        <textarea
          class="w-full my-2 border rounded px-2"
          placeholder="Message"
        />
        <button
          class="border rounded w-full p-1 bg-blue-500 text-white font-medium"
        >
          Send
        </button>
      </div>
    </div>
  </div>
</template>

<script>
// import Portal from "../../components/portal";

export default {
  components: {
    // Portal,
  },
};
</script>

<style></style>
