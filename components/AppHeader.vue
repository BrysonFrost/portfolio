<script setup>
  const route = useRoute();
  const router = useRouter();

  //when page changes, close navbar
  router.beforeEach(() => {
    var navCollapse = document.getElementById('navbarNav');
    if(navCollapse.classList.contains('show')) {
      navCollapse.classList.remove('show');
    }  

  })
</script>


<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark mb-3 sticky-top">
    <div class="container">
      <NuxtLink to="/" class="navbar-brand text-light">LOGO</NuxtLink>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
        aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <NuxtLink to="/" class="nav-link" active-class="active">Home</NuxtLink>
          </li>
          <li class="nav-item">
            <NuxtLink to="/about" class="nav-link" active-class="active">About</NuxtLink>
          </li>
          <li class="nav-item">
            <NuxtLink to="/projects" class="nav-link" active-class="active">Projects</NuxtLink>
          </li>
          <li class="nav-item">
            <NuxtLink to="/blog" class="nav-link" active-class="active">Blog Posts</NuxtLink>
          </li>
          <li class="nav-item">
            <NuxtLink to="/contact" class="nav-link" active-class="active">Contact</NuxtLink>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>