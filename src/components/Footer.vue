<template>
  <footer class="app-footer">
    <div class="container app-footer__inner surface">
      <div class="app-footer__left">
        <div class="mono muted">© {{ year }} Markus Olsson</div>
        <small class="muted">Built with Vue • Designed with care</small>
      </div>

      <div class="app-footer__right">
        <a
          class="btn btn--ghost"
          href="https://github.com/FeodalherreN/markusolsson.com"
          target="_blank"
          rel="noreferrer"
        >
          GitHub
        </a>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return { year: new Date().getFullYear() };
  },
};
</script>

<style scoped>
.app-footer {
  padding: 26px 0 34px;
}
.app-footer__inner {
  padding: 16px 18px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 16px;
}
.app-footer__left small {
  display: block;
  margin-top: 4px;
}
@media (max-width: 640px) {
  .app-footer__inner {
    flex-direction: column;
    text-align: center;
  }
}
</style>
