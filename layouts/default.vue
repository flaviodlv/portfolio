<script setup>
defineOptions({ name: 'DefaultLayout' })
</script>

<template>
  <div class="layout">
    <nav class="navbar">
      <div class="navbar-brand">
        <NuxtLink to="/" aria-label="Home">
          <svg viewBox="0 0 24 24" width="32" height="32" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M3 10.5L12 3l9 7.5V21a1 1 0 0 1-1 1h-5v-6H9v6H4a1 1 0 0 1-1-1V10.5Z" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </NuxtLink>
      </div>
      <ul class="navbar-links">
        <li><NuxtLink to="/projets">Projets</NuxtLink></li>
        <li><NuxtLink to="/entreprise">Entreprise</NuxtLink></li>
        <li><NuxtLink to="/cv">CV</NuxtLink></li>
        <li><NuxtLink to="/veille">Veille Technologique</NuxtLink></li>
      </ul>
    </nav>

    <main class="content">
      <slot />
    </main>
  </div>
</template>

<style>
html, body {
  margin: 0;
  padding: 0;
}

* {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
}


.layout {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.content {
  flex: 1;
}


.navbar {
  display: flex;
  align-items: center;
  justify-content: space-around;
  background: white;
  padding: 0.6rem;
}

.navbar-brand a {
  color: #000000;
  font-size: 1.6rem;
  text-decoration: none;
  margin-left: 5rem;
  transition: color 0.3s;
}

.navbar-brand a:hover {
  color: #58a6ff;
}

.navbar-links {
  display: flex;
  gap: 2.8rem;
  list-style: none;
}

.navbar-links li a {
  color: #000000;
  text-decoration: none;
  font-size: 1.1rem;
  transition: color 0.3s;
}

.navbar-links li a:hover {
  color: #58a6ff;
}
</style>
