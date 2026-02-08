<template>
  <div id="app" class="app">
    <!-- Decorative background -->
    <div class="bg-grid" aria-hidden="true"></div>
    <div class="bg-glow bg-glow--a" aria-hidden="true"></div>
    <div class="bg-glow bg-glow--b" aria-hidden="true"></div>

    <GithubLink />
    <Header />

    <main class="page">
      <About />
      <Experience />
    </main>

    <Footer />
  </div>
</template>

<script>
import About from "./components/About.vue";
import Experience from "./components/Experience.vue";
import Footer from "./components/Footer.vue";
import Header from "./components/Header.vue";
import GithubLink from "./components/GithubLink.vue";

export default {
  name: "App",
  components: { About, Experience, Footer, Header, GithubLink },
};
</script>

<style>
/* Kept for backwards compatibility (older components used .card) */
.card {
  border-radius: var(--radius-lg);
  padding: 22px;
  background: var(--surface);
  border: 1px solid var(--border);
  box-shadow: var(--shadow);
}
</style>
