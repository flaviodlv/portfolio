<template>
  <div class="home-page">
    <section class="hero">
      <div class="hero-inner">
        <p class="hero-eyebrow">Accueil</p>
        <h1 class="hero-name">Flavio DE OLIVEIRA</h1>
        <p class="hero-role">
          Étudiant BTS SIO &bull; Développeur Informatique en alternance
        </p>
        <div class="hero-contact">
          <p>06 09 01 56 07</p>
          <span class="dot"></span>
          <a href="mailto:dolv.flavio@gmail.com">dolv.flavio@gmail.com</a>
        </div>
      </div>
      <div class="hero-line"></div>
    </section>

    <section class="about">
      <div class="about-grid">
        <div class="about-block">
          <h2>Ma passion</h2>
          <p>
            J'aime travailler sur des interfaces modernes, propres et
            ergonomiques. J'accorde beaucoup d'importance à la qualité du code,
            à l'optimisation et à l'expérience utilisateur.
          </p>
        </div>
        <div class="about-block">
          <h2>Mes projets</h2>
          <p>
            Sur ce portfolio, vous trouverez mes différents projets — réalisés
            en cours, en entreprise ou durant mon temps libre. Mon objectif :
            progresser en continu, apprendre de nouvelles technologies et
            construire des solutions utiles.
          </p>
        </div>
      </div>
    </section>

    <section class="cta">
      <NuxtLink to="/projets" class="cta-btn">
        Voir mes projets
        <svg
          viewBox="0 0 20 20"
          width="16"
          height="16"
          fill="none"
          stroke="currentColor"
          stroke-width="1.8"
        >
          <path
            d="M4 10h12M11 5l5 5-5 5"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
        </svg>
      </NuxtLink>
    </section>
  </div>
</template>

<script setup>
defineOptions({ name: "HomePage" });
</script>

<style scoped>
.home-page {
  padding-top: 0;
}

.hero {
  padding: 96px 72px 0;
  max-width: 960px;
  margin: 0 auto;
}

.hero-eyebrow {
  font-size: 0.75rem;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  color: var(--muted);
  font-weight: 500;
  margin-bottom: 28px;
}

.hero-name {
  font-size: clamp(3rem, 8vw, 5.5rem);
  font-weight: 300;
  line-height: 1.05;
  color: var(--ink);
  margin-bottom: 28px;
  letter-spacing: -0.02em;
}

.hero-role {
  font-size: 1rem;
  color: var(--muted);
  font-weight: 400;
  margin-bottom: 20px;
}

.hero-contact {
  display: flex;
  align-items: center;
  gap: 14px;
  flex-wrap: wrap;
}

.hero-contact a {
  color: var(--muted);
  text-decoration: none;
  font-size: 1rem;
  transition: color 0.2s;
}
.hero-contact a:hover {
  color: var(--ink);
}

.hero-contact p {
  color: var(--muted);
  text-decoration: none;
  font-size: 1rem;
  transition: color 0.2s;
}

.dot {
  width: 3px;
  height: 3px;
  border-radius: 50%;
  background: #cccccc;
  display: inline-block;
}

.hero-line {
  height: 1px;
  background: var(--border);
  margin-top: 72px;
}

.about {
  max-width: 960px;
  margin: 0 auto;
  padding: 72px 72px;
}

.about-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 48px;
}

.about-block {
  display: flex;
  flex-direction: column;
  gap: 16px;
}

.about-block h2 {
  font-size: 1.2rem;
  font-weight: 500;
  color: var(--ink);
  letter-spacing: -0.01em;
}

.about-block p {
  font-size: 0.925rem;
  color: var(--muted);
  line-height: 1.8;
}

.cta {
  max-width: 960px;
  margin: 0 auto;
  padding: 48px 72px 96px;
  display: flex;
  align-items: center;
  gap: 32px;
  border-top: 1px solid var(--border);
}

.cta-label {
  font-size: 0.78rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--muted);
}

.cta-btn {
  display: inline-flex;
  align-items: center;
  gap: 10px;
  padding: 12px 28px;
  background: var(--ink);
  color: #ffffff;
  text-decoration: none;
  font-size: 0.875rem;
  font-weight: 400;
  letter-spacing: 0.02em;
  transition: background 0.2s;
}
.cta-btn:hover {
  background: #333333;
}

@media (max-width: 768px) {
  .hero {
    padding: 60px 24px 0;
  }
  .hero-name {
    font-size: 2.6rem;
  }
  .about {
    padding: 48px 24px;
  }
  .about-grid {
    grid-template-columns: 1fr;
    gap: 36px;
  }
  .cta {
    padding: 36px 24px 60px;
    flex-direction: column;
    align-items: flex-start;
    gap: 20px;
  }
}
</style>
