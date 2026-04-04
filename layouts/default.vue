<script setup>
defineOptions({ name: 'DefaultLayout' })
</script>

<template>
  <div class="layout">
    <nav class="navbar">
      <div class="navbar-brand">
        <NuxtLink to="/">Flavio De Oliveira</NuxtLink>
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
