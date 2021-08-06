<template>
  <div class="gradient app-header d-flex align-items-center">
    <div class="container">
      <div class="row d-flex align-items-center">
        <div class="col-md-5 col-sm-12 mb-3">
          <img
            src="../assets/portrait.png"
            class="rounded-circle mx-auto d-block profile-picture"
            alt="Profile picture"
          />
        </div>
        <div class="col-md-7 col-sm-12 text-center text-white">
          <h2>Markus Olsson</h2>
          <h3 class="py-2">Software Engineer</h3>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style lang="scss" scoped>
.app-header {
  height: 400px;
}

.profile-picture {
  max-width: 200px;
  max-height: 400px;
}
</style>
