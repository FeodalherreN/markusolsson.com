<template>
  <section id="about" class="section">
    <div class="container">
      <div class="surface surface--hover about">
        <div class="about__inner">
          <h2 class="header">Who am I?</h2>

          <p class="muted">
            I’m a developer who enjoys going deep in the jungle of tech — but I
            also care a lot about <span class="mono">UX</span>,
            <span class="mono">design systems</span>, and shipping work that
            feels polished.
          </p>

          <p class="muted">
            Professionally I do web development, but I don’t like to limit
            myself to any specific technology or side of the stack. On my spare
            time I like to hit the gym, go on afterworks, and learn new things.
            My newest passion is
            <a href="https://www.rust-lang.org/" target="_blank" rel="noreferrer">Rust</a>.
          </p>

          <div class="about__chips" aria-label="Highlights">
            <span class="badge"><span class="badge__spark"></span>Frontend</span>
            <span class="badge"><span class="badge__spark"></span>Backend</span>
            <span class="badge"><span class="badge__spark"></span>Cloud</span>
            <span class="badge"><span class="badge__spark"></span>Design-minded</span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default { name: "About" };
</script>

<style scoped>
.about {
  padding: 22px;
}
.about__inner {
  padding: 8px 6px;
}
.about__chips {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin-top: 14px;
}
</style>
