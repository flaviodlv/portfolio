<template>
  <div class="projets-page">
    <div class="page-inner">
      <header class="page-header">
        <p class="eyebrow">Projets</p>
        <h1>Mes Projets</h1>
        <p class="subtitle">Réalisations et expérimentations</p>
      </header>

      <div class="divider"></div>

      <section class="project-section">
        <h2 class="section-label">
          <span class="label-num">01</span> Projets scolaires
        </h2>
        <div class="project-list">
          <article class="project-card">
            <div class="project-meta">
              <span class="project-tag">PPE 1</span>
              <span class="project-year">2024</span>
            </div>
            <h3>Site web de e-commerce</h3>
            <p>
              Projet Professionnel Encadré réalisé en première année —
              conception et développement d'une boutique en ligne spécialisée
              dans la vente d'ordinateurs.
            </p>
            <a
              href="https://drive.google.com/drive/folders/1H8juEu5YwMbv43fnoOrz8SF_Hb0wnFGV"
              target="_blank"
              class="project-link"
            >
              Documentation
              <svg
                viewBox="0 0 16 16"
                width="13"
                height="13"
                fill="none"
                stroke="currentColor"
                stroke-width="1.8"
              >
                <path
                  d="M3 8h10M8 3l5 5-5 5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg>
            </a>
          </article>

          <article class="project-card">
            <div class="project-meta">
              <span class="project-tag">PPE 2</span>
              <span class="project-year">2025</span>
            </div>
            <h3>Application Windows de gestion d'interventions</h3>
            <p>
              Projet Professionnel Encadré réalisé en deuxième année —
              application logiciel permettant de créer et gérer des
              interventions sur des produits.
            </p>
            <a
              href="https://drive.google.com/drive/folders/1qDKq8KDi-vJNLCOoh4nnSDBB5a77C_tP"
              target="_blank"
              class="project-link"
            >
              Documentation
              <svg
                viewBox="0 0 16 16"
                width="13"
                height="13"
                fill="none"
                stroke="currentColor"
                stroke-width="1.8"
              >
                <path
                  d="M3 8h10M8 3l5 5-5 5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg>
            </a>
          </article>
        </div>
      </section>

      <div class="divider"></div>

      <section class="project-section">
        <h2 class="section-label">
          <span class="label-num">02</span> Projets personnels
        </h2>
        <div class="project-list">
          <article class="project-card wide">
            <h3>Projets extra-scolaires</h3>
            <p>
              Collection de projets réalisés en dehors du cadre scolaire — jeux
              et autres.
            </p>
            <a
              href="https://github.com/flaviodlv/"
              target="_blank"
              class="project-link"
            >
              Voir les projets sur Github
              <svg
                viewBox="0 0 16 16"
                width="13"
                height="13"
                fill="none"
                stroke="currentColor"
                stroke-width="1.8"
              >
                <path
                  d="M3 8h10M8 3l5 5-5 5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg>
            </a>
          </article>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
definePageMeta({ layout: "default" });
</script>

<style scoped>
.projets-page {
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

.project-section {
  padding: 56px 0;
}

.section-label {
  display: flex;
  align-items: baseline;
  gap: 12px;
  font-size: 0.72rem;
  font-weight: 500;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--muted);
  margin-bottom: 36px;
}

.label-num {
  color: var(--ink);
}

.project-list {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 1px;
  background: var(--border);
  border: 1px solid var(--border);
}

.project-card {
  background: #ffffff;
  padding: 36px 32px;
  display: flex;
  flex-direction: column;
  gap: 12px;
  transition: background 0.2s;
}
.project-card:hover {
  background: #fafafa;
}
.project-card.wide {
  grid-column: 1 / -1;
}

.project-meta {
  display: flex;
  align-items: center;
  gap: 12px;
}

.project-tag {
  font-size: 0.7rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  font-weight: 500;
  color: var(--ink);
  background: rgba(0, 0, 0, 0.06);
  padding: 3px 8px;
  border-radius: 2px;
}

.project-year {
  font-size: 0.75rem;
  color: var(--muted);
}

.project-card h3 {
  font-size: 1.15rem;
  font-weight: 500;
  color: var(--ink);
  line-height: 1.3;
  letter-spacing: -0.01em;
}

.project-card p {
  font-size: 0.9rem;
  color: var(--muted);
  line-height: 1.75;
  flex: 1;
}

.project-link {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  font-size: 0.8rem;
  font-weight: 500;
  color: var(--ink);
  text-decoration: none;
  border-bottom: 1px solid var(--ink);
  padding-bottom: 1px;
  width: fit-content;
  margin-top: 8px;
  transition: opacity 0.2s;
}
.project-link:hover {
  opacity: 0.5;
}

@media (max-width: 768px) {
  .page-inner {
    padding: 0 24px;
  }
  .project-list {
    grid-template-columns: 1fr;
  }
  .project-card.wide {
    grid-column: 1;
  }
}
</style>
