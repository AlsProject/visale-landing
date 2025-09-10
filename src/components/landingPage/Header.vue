<template>
  <header class="header">
    <nav class="navbar navbar-expand-lg navbar-light fixed-top bg-white shadow-sm">
      <div class="container">
        <!-- Logo -->
        <a class="navbar-brand d-flex align-items-center" href="#">
          <img src="/img/logo.svg" alt="Visale" height="50" class="me-2">
        </a>

        <!-- Mobile Toggle Button -->
        <button 
          class="navbar-toggler" 
          type="button" 
          data-bs-toggle="collapse" 
          data-bs-target="#navbarNav"
          aria-controls="navbarNav" 
          aria-expanded="false" 
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>

        <!-- Navigation Links
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav ms-auto me-3">
            <li class="nav-item">
              <a class="nav-link" href="#accueil">Accueil</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#why-choose-us">Pourquoi Visale</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#who-can-apply">Qui peut postuler</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#contact">Contact</a>
            </li>
          </ul>
        </div> -->
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style scoped>
.header {
  /* Styles personnalisés si nécessaires */
}

.navbar-brand {
  color: #1f2937 !important;
}

.nav-link {
  color: #6b7280 !important;
  font-weight: 500;
  transition: color 0.2s ease;
}

.nav-link:hover {
  color: #3b82f6 !important;
}
</style>
