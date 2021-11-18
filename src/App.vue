<template>
  <About />
  <div class="border-t mx-2" />
  <ProvidingServices />
  <div class="border-t mx-2" />
  <Blogs />
  <div class="border-t mx-2" />
  <Support />
</template>

<script>
import About from "./pages/About";
import Blogs from "./pages/Blogs";
import ProvidingServices from "./pages/ProvidingServices";
import Support from "./pages/Support";

export default {
  name: "App",
  components: {
    About,
    ProvidingServices,
    Blogs,
    Support,
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
  margin-top: 60px;
}
</style>
