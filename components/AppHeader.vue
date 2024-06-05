<template>
  <nav class="navbar navbar-expand-lg bg-dark bg-gradient mb-3">
  <div class="container">
    <NuxtLink to="/" class="navbar-brand text-light">LOGO</NuxtLink>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
      <ul class="navbar-nav">
        <li class="nav-item">
          <NuxtLink to="/" class="nav-link text-light">Home</NuxtLink>
        </li>
        <li class="nav-item">
          <NuxtLink to="/about" class="nav-link text-light">About</NuxtLink>
        </li>
        <li class="nav-item">
          <NuxtLink to="/projects" class="nav-link text-light">Projects</NuxtLink>
        </li>
        <li class="nav-item">
          <NuxtLink to="/about" class="nav-link text-light">Blog Posts</NuxtLink>
        </li>
        <li class="nav-item">
          <NuxtLink to="/about" class="nav-link text-light">Contact</NuxtLink>
        </li>
      </ul>
    </div>
  </div>
</nav>
</template>