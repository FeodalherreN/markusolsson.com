<template>
  <header class="hero">
    <div class="container hero__inner">
      <div class="hero__card surface">
        <div class="hero__grid">
          <div class="hero__media">
            <img
              src="../assets/portrait.png"
              class="profile-picture"
              alt="Profile picture"
            />
            <div class="profile-ring" aria-hidden="true"></div>
          </div>

          <div class="hero__content">
            <div class="kicker">
              <span class="kicker__dot"></span>
              <span class="mono">console.log</span>
              <span class="muted">( "hello" )</span>
            </div>

            <h1 class="hero__title">Markus Olsson</h1>
            <p class="hero__subtitle">Software Engineer</p>

            <p class="hero__blurb muted">
              I build reliable products with a soft spot for clean architecture,
              performance, and delightful UI details.
            </p>

            <div class="hero__cta">
              <a class="btn btn--primary" href="#experience">View experience</a>
              <a class="btn btn--ghost" href="#about">About me</a>
            </div>

            <div class="hero__terminal" aria-hidden="true">
              <span class="mono">$</span>
              <span class="mono"> npm run build</span>
              <span class="cursor"></span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default { name: "Header" };
</script>

<style lang="scss" scoped>
.hero {
  padding: 40px 0 10px;
}

.hero__inner {
  padding-top: 16px;
}

.hero__card {
  padding: 26px;
}

.hero__grid {
  display: grid;
  grid-template-columns: 220px 1fr;
  gap: 26px;
  align-items: center;
}

.hero__media {
  position: relative;
  display: grid;
  place-items: center;
  padding: 10px;
}

.profile-picture {
  width: 190px;
  height: 190px;
  border-radius: 999px;
  object-fit: cover;
  border: 1px solid rgba(255, 255, 255, 0.16);
  box-shadow: 0 18px 50px rgba(0, 0, 0, 0.42);
}

.profile-ring {
  position: absolute;
  inset: -8px;
  border-radius: 999px;
  border: 1px solid rgba(87, 226, 229, 0.22);
  box-shadow: 0 0 0 8px rgba(87, 226, 229, 0.06);
  pointer-events: none;
}

.hero__title {
  font-size: clamp(34px, 4vw, 48px);
  line-height: 1.05;
  margin-top: 12px;
}

.hero__subtitle {
  margin-top: 8px;
  font-weight: 600;
  color: rgba(255, 255, 255, 0.78);
}

.hero__blurb {
  margin-top: 14px;
  max-width: 56ch;
}

.hero__cta {
  margin-top: 18px;
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
}

.hero__terminal {
  margin-top: 16px;
  padding: 10px 12px;
  width: fit-content;
  border-radius: 12px;
  border: 1px solid rgba(255, 255, 255, 0.12);
  background: rgba(0, 0, 0, 0.22);
  color: rgba(255, 255, 255, 0.78);
}

.cursor {
  display: inline-block;
  width: 10px;
  height: 16px;
  margin-left: 6px;
  background: rgba(87, 226, 229, 0.85);
  border-radius: 2px;
  vertical-align: -2px;
  animation: blink 1.05s steps(1) infinite;
}

@keyframes blink {
  50% { opacity: 0; }
}

@media (max-width: 768px) {
  .hero__grid {
    grid-template-columns: 1fr;
    text-align: center;
  }
  .hero__terminal { margin-left: auto; margin-right: auto; }
  .hero__cta { justify-content: center; }
}
</style>
