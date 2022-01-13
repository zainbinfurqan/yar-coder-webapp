<template>
  <div id="popup-target" class="min-h-14"></div>
  <!-- <About /> -->
  <!-- <div class="border-t mx-2" /> -->
  <!-- <ProvidingServices /> -->
  <!-- <div class="border-t mx-2" /> -->
  <Socials />
  <Blogs />
  <Videos />
  <!-- <div class="border-t mx-2" /> -->
  <!-- <Support /> -->
  <!-- <div class="border-t mx-2" /> -->
  <!-- <UnderConstruction /> -->
  <!-- <Contact /> -->
</template>

<script>
import Videos from "./pages/Videos";
import Blogs from "./pages/Blogs";
import Socials from "./pages/Socials";
// import Support from "./pages/Support";
// import Contact from "./pages/Contact";
// import UnderConstruction from "./pages/UnderConstruction";

export default {
  name: "App",
  components: {
    Videos,
    Socials,
    Blogs,
    // Support,
    // Contact,
    // UnderConstruction,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0px;
}
</style>
