<script setup>

</script>

<template>
  <nav class="navbar navbar-expand-lg navbar-light py-3">
    <div class="container px-5">
      <RouterLink to="/" class="navbar-brand">
        <span class="fw-bolder text-gradient fs-4">@ummimuyasaroh
        </span>
      </RouterLink>
      <a class="navbar-toggler" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <i class='bx bx-menu-alt-right'></i>
      </a>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav ms-auto mb-2 mb-lg-0 small fw-bolder">
          <li class="nav-item"><RouterLink to="/" class="nav-link">Home</RouterLink></li>
          <li class="nav-item"><RouterLink to="/resume" class="nav-link">Resume</RouterLink></li>
          <li class="nav-item"><RouterLink to="/project" class="nav-link">Projects</RouterLink></li>
          <li class="nav-item"><RouterLink to="/contact" class="nav-link">Contact</RouterLink></li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<style scoped>
.navbar-toggler {
  border: none !important;
  font-size: 24px !important;
}
</style>