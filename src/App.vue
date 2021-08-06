<template>
  <div id="app" class="app h-100">
    <Header />
    <GithubLink />
    <About />
  </div>
</template>

<script>
import About from "./components/About.vue";
import Header from "./components/Header.vue";
import GithubLink from "./components/GithubLink.vue";
export default {
  name: "App",
  components: {
    About,
    Header,
    GithubLink,
  },
};
</script>

<style>
.card {
  padding: 20px 20px;
  color: white;
  background-color: black;
  opacity: 0.6;
  -moz-box-shadow: 0 0 30px black;
  -webkit-box-shadow: 0 0 30px black;
  box-shadow: 0 0 30px black;
}
</style>
