<template>
  <div class="entreprise-page">
    <div class="page-inner">
      <header class="page-header">
        <p class="eyebrow">Entreprise</p>
        <h1>Hachette Livre</h1>
        <p class="subtitle">Mon expérience chez eux</p>
      </header>

      <div class="divider"></div>

      <section class="entreprise-body">
        <div class="entreprise-info">
          <p>
            Cette section présente mon expérience d'alternance chez <strong>Hachette</strong>,
            mes missions, les technologies utilisées au sein de l'entreprise.
          </p>
          <a href="https://gamma.app/docs/Hachette-Livre-9lzcj7oyhqjyra3?mode=doc" target="_blank"
            rel="noopener noreferrer" class="entreprise-link">
            Voir le diaporama
          </a>
          <a 
            href="/Diapo.pdf" 
            download 
            class="entreprise-link secondary"
          >
            Télécharger le PDF
          </a>
        </div>

        <div class="company-card">
          <div class="company-header">
            <img
              src="https://upload.wikimedia.org/wikipedia/en/thumb/9/9b/Hachette_logo.svg/3840px-Hachette_logo.svg.png"
              alt="Hachette logo" class="company-logo" />
          </div>
          <span class="company-sector">Édition &amp; Médias</span>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
definePageMeta({ layout: 'default' })
</script>

<style scoped>
.entreprise-page {
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

.entreprise-body {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 64px;
  padding: 64px 0;
  align-items: start;
}

.badge-coming {
  display: inline-block;
  font-size: 0.7rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  font-weight: 500;
  color: var(--muted);
  background: rgba(0, 0, 0, 0.06);
  padding: 4px 10px;
  border-radius: 2px;
  margin-bottom: 24px;
}

.entreprise-info p {
  font-size: 0.925rem;
  color: var(--muted);
  line-height: 1.8;
  margin-bottom: 12px;
}

.entreprise-info strong {
  color: var(--ink);
  font-weight: 500;
}

.company-card {
  border: 1px solid var(--border);
  padding: 36px 32px;
  display: flex;
  flex-direction: column;
  gap: 10px;
}

.company-label {
  font-size: 0.7rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--muted);
  font-weight: 500;
}

.company-name {
  font-size: 2.2rem;
  font-weight: 300;
  color: var(--ink);
  line-height: 1;
  letter-spacing: -0.02em;
  margin: 0;
}

.company-header {
  display: flex;
  align-items: center;
  gap: 16px;
}

.company-logo {
  height: 60px;
  width: auto;
  object-fit: contain;
}

.company-sector {
  font-size: 0.85rem;
  color: var(--muted);
}

.entreprise-link {
  display: inline-flex;
  align-items: center;
  gap: 10px;
  padding: 13px 28px;
  background: var(--ink);
  color: #ffffff;
  text-decoration: none;
  font-size: 0.875rem;
  transition: background 0.2s;
  margin-top: 10px;
  margin-right: 10px;
}

.entreprise-link:hover {
  background: #555555;
}

.entreprise-link.secondary {
  background: #888;
}

@media (max-width: 768px) {
  .page-inner {
    padding: 0 24px;
  }

  .entreprise-body {
    grid-template-columns: 1fr;
    gap: 40px;
  }
}
</style>