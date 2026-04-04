<template>
  <div class="cv-page">
    <div class="page-inner">
      <header class="page-header">
        <p class="eyebrow">CV</p>
        <h1>Curriculum Vitae</h1>
        <p class="subtitle">Mon parcours et mes compétences</p>
      </header>

      <div class="divider"></div>

      <section class="cv-body">
        <div class="cv-info">
          <p>
            Le CV complet est disponible en cliquant sur le lien ci-dessous. Il
            regroupe mon parcours scolaire, mes expériences en alternance et mes
            compétences techniques.
          </p>
          <a href="/CV.pdf" target="_blank" class="cv-download-btn">
            Voir le CV complet
          </a>
        </div>

        <div class="cv-highlights">
          <div class="highlight-item">
            <span class="h-label">Formation</span>
            <span class="h-value">BTS SIO — option SLAM</span>
          </div>
          <div class="highlight-item">
            <span class="h-label">Statut</span>
            <span class="h-value">Alternant — Développeur</span>
          </div>
          <div class="highlight-item">
            <span class="h-label">Entreprise</span>
            <span class="h-value">Hachette Livre</span>
          </div>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
definePageMeta({ layout: "default" });
</script>

<style scoped>
.cv-page {
  min-height: 100vh;
  padding-bottom: 96px;
}

.page-inner {
  max-width: 960px;
  margin: 0 auto;
  padding: 0 72px;
}

.page-header {
  padding-top: 72px;
  padding-bottom: 48px;
}

.eyebrow {
  font-size: 0.75rem;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  color: var(--muted);
  font-weight: 500;
  margin-bottom: 20px;
}

.page-header h1 {
  font-size: clamp(2.2rem, 5vw, 3.5rem);
  font-weight: 300;
  color: var(--ink);
  margin-bottom: 12px;
  letter-spacing: -0.02em;
}

.subtitle {
  color: var(--muted);
  font-size: 0.95rem;
}

.divider {
  height: 1px;
  background: var(--border);
}

.cv-body {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 64px;
  padding: 64px 0;
}

.cv-info p {
  font-size: 0.925rem;
  color: var(--muted);
  line-height: 1.8;
  margin-bottom: 32px;
}

.cv-download-btn {
  display: inline-flex;
  align-items: center;
  gap: 10px;
  padding: 13px 28px;
  background: var(--ink);
  color: #ffffff;
  text-decoration: none;
  font-size: 0.875rem;
  transition: background 0.2s;
}
.cv-download-btn:hover {
  background: #555555;
}

.cv-highlights {
  display: flex;
  flex-direction: column;
  border-top: 1px solid var(--border);
}

.highlight-item {
  display: flex;
  justify-content: space-between;
  align-items: baseline;
  padding: 18px 0;
  border-bottom: 1px solid var(--border);
}

.h-label {
  font-size: 0.72rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--muted);
  font-weight: 500;
}

.h-value {
  font-size: 0.9rem;
  color: var(--ink);
}

.h-value a {
  color: var(--ink);
  text-decoration: none;
  border-bottom: 1px solid var(--border);
  transition: opacity 0.2s;
}
.h-value a:hover {
  opacity: 0.5;
}

@media (max-width: 768px) {
  .page-inner {
    padding: 0 24px;
  }
  .cv-body {
    grid-template-columns: 1fr;
    gap: 40px;
  }
}
</style>
