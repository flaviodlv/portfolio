<template>
  <div>
    <nav class="navbar">
      <div class="navbar-brand">
        <NuxtLink to="/">Flavio De Oliveira</NuxtLink>
      </div>
      <ul class="navbar-links">
        <li>
          <NuxtLink to="/projets">Projets</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/entreprise">Entreprise</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/cv">CV</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/veille">Veille Technologique</NuxtLink>
        </li>
      </ul>
    </nav>
  </div>
  <slot />
</template>

<script setup></script>

<style>
html,
body {
  margin: 0;
  padding: 0;
}

* {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
}

.navbar {
  display: flex;
  align-items: center;
  justify-content: space-around;
  background: linear-gradient(135deg, #0d1117 0%, #161b22 100%);
  padding: 0.6rem;
  position: relative;
}

.navbar-brand a {
  color: #fff;
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
  color: #fff;
  text-decoration: none;
  font-size: 1.1rem;
  transition: color 0.3s;
}

.navbar-links li a:hover {
  color: #58a6ff;
}
</style>
