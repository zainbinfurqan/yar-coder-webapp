<template>
  <About />
  <Blogs />
</template>

<script>
import About from "./pages/About";
import Blogs from "./pages/Blogs";

export default {
  name: "App",
  components: {
    About,
    Blogs,
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
