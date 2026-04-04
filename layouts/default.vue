<script setup>
defineOptions({ name: "DefaultLayout" });
</script>

<template>
  <div class="layout">
    <nav class="navbar">
      <NuxtLink to="/" class="navbar-brand" aria-label="Accueil">
        <span class="brand-initials">FD</span>
      </NuxtLink>
      <ul class="navbar-links">
        <li><NuxtLink to="/projets">Projets</NuxtLink></li>
        <li><NuxtLink to="/entreprise">Entreprise</NuxtLink></li>
        <li><NuxtLink to="/cv">CV</NuxtLink></li>
        <li><NuxtLink to="/veille">Veille</NuxtLink></li>
      </ul>
      <button
        class="nav-toggle"
        aria-label="Menu"
        @click="menuOpen = !menuOpen"
      >
        <span></span><span></span><span></span>
      </button>
    </nav>
    <div class="mobile-menu" :class="{ open: menuOpen }">
      <ul>
        <li>
          <NuxtLink to="/projets" @click="menuOpen = false">Projets</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/entreprise" @click="menuOpen = false"
            >Entreprise</NuxtLink
          >
        </li>
        <li><NuxtLink to="/cv" @click="menuOpen = false">CV</NuxtLink></li>
        <li>
          <NuxtLink to="/veille" @click="menuOpen = false">Veille</NuxtLink>
        </li>
      </ul>
    </div>
    <main class="content">
      <slot />
    </main>
  </div>
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=DM+Sans:wght@300;400;500&display=swap");

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

html,
body {
  background: #ffffff;
  color: #111111;
  font-family: "DM Sans", sans-serif;
  font-weight: 400;
  -webkit-font-smoothing: antialiased;
  overflow: hidden;
}

:root {
  --accent: #111111;
  --accent-hover: #333333;
  --ink: #111111;
  --muted: #888888;
  --surface: #ffffff;
  --bg: #ffffff;
  --border: rgba(0, 0, 0, 0.1);
  --nav-h: 64px;
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
  position: sticky;
  top: 0;
  z-index: 100;
  height: var(--nav-h);
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 150px;
  background: rgba(235, 235, 235, 0.4);
  backdrop-filter: blur(12px);
  border-bottom: 1px solid var(--border);
}

.navbar-brand {
  text-decoration: none;
  display: flex;
  align-items: center;
}

.brand-initials {
  font-family: "DM Serif Display", serif;
  font-size: 1.4rem;
  color: var(--ink);
  letter-spacing: 0.02em;
  transition: color 0.1s;
}

.brand-initials:hover {
  color: var(--accent);
}

.navbar-links {
  display: flex;
  gap: 2.4rem;
  list-style: none;
}

.navbar-links li a {
  color: var(--muted);
  text-decoration: none;
  font-size: 0.875rem;
  font-weight: 400;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  transition: color 0.2s;
  position: relative;
  padding-bottom: 2px;
}

.navbar-links li a::after {
  content: "";
  position: absolute;
  bottom: -2px;
  left: 0;
  width: 0;
  height: 1px;
  background: var(--accent);
  transition: width 0.25s ease;
}

.navbar-links li a:hover,
.navbar-links li a.router-link-active {
  color: var(--ink);
}

.navbar-links li a.router-link-active::after,
.navbar-links li a:hover::after {
  width: 100%;
}

.nav-toggle {
  display: none;
  flex-direction: column;
  gap: 5px;
  background: none;
  border: none;
  cursor: pointer;
  padding: 4px;
}

.nav-toggle span {
  display: block;
  width: 22px;
  height: 1.5px;
  background: var(--ink);
  transition: all 0.3s;
}

/* Mobile menu */
.mobile-menu {
  display: none;
  position: fixed;
  top: var(--nav-h);
  left: 0;
  right: 0;
  background: #ffffff;
  border-bottom: 1px solid var(--border);
  z-index: 99;
  transform: translateY(-100%);
  opacity: 0;
  transition:
    transform 0.3s ease,
    opacity 0.3s ease;
}

.mobile-menu.open {
  transform: translateY(0);
  opacity: 1;
}

.mobile-menu ul {
  list-style: none;
  padding: 16px 24px 24px;
}

.mobile-menu ul li a {
  display: block;
  padding: 12px 0;
  color: var(--ink);
  text-decoration: none;
  font-size: 1.1rem;
  border-bottom: 1px solid var(--border);
}
</style>
