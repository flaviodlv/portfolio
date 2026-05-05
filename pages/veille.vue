<template>
  <div class="veille-page">
    <div class="page-inner">
      <header class="page-header">
        <p class="eyebrow">Veille</p>
        <h1>Veille Technologique</h1>
        <p class="subtitle">Suivi de l'actualité et des tendances</p>
      </header>

      <div class="divider"></div>

      <section class="veille-body">
        <div class="veille-intro">
          <div class="badge-coming">DLSS</div>
          <p>
            Cette section présente ma veille technologique — les sujets que je
            suis, et les sources.
          </p>

          <!-- Bouton Gamma -->
          <a 
            href="https://gamma.app/docs/Untitled-rxsyzp9rvcto7us?mode=doc" 
            target="_blank" 
            class="veille-link"
          >
            Accéder à la veille
          </a>

          <!-- Bouton téléchargement -->
          <a 
            href="/Veille.pdf" 
            download 
            class="veille-link secondary"
          >
            Télécharger le PDF
          </a>
        </div>

        <div class="topics-preview">
          <p class="topics-label">Thèmes explorés</p>
          <ul class="topics-list">
            <li>Sécurité applicative</li>
            <li>Frameworks JavaScript modernes</li>
            <li>Intelligence artificielle &amp; LLMs</li>
          </ul>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
definePageMeta({ layout: "default" });
</script>

<style scoped>
.veille-page {
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

.veille-body {
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

.veille-intro p {
  font-size: 0.925rem;
  color: var(--muted);
  line-height: 1.8;
  margin-bottom: 28px;
}

.veille-link {
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

.veille-link:hover {
  background: #555555;
}

.veille-link.secondary {
  background: #888;
}

.topics-label {
  font-size: 0.7rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--muted);
  font-weight: 500;
  margin-bottom: 20px;
}

.topics-list {
  list-style: none;
  border-top: 1px solid var(--border);
}

.topics-list li {
  font-size: 0.9rem;
  color: var(--ink);
  padding: 16px 0;
  border-bottom: 1px solid var(--border);
  display: flex;
  align-items: center;
  gap: 12px;
}

.topics-list li::before {
  content: "";
  display: inline-block;
  width: 4px;
  height: 4px;
  border-radius: 50%;
  background: var(--muted);
  flex-shrink: 0;
}

/* PDF viewer */
.pdf-viewer {
  margin-top: 32px;
  border: 1px solid var(--border);
}

.pdf-fallback {
  font-size: 0.8rem;
  color: var(--muted);
  padding: 10px;
}

/* Responsive */
@media (max-width: 768px) {
  .page-inner {
    padding: 0 24px;
  }

  .veille-body {
    grid-template-columns: 1fr;
    gap: 40px;
  }
}
</style>