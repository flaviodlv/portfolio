<template>
  <div class="home-page">
    <div class="container">
      <div class="hero-section">
        <h1 class="hero-title">
          <span class="name">Flavio DE OLIVEIRA</span>
        </h1>
        <p class="hero-subtitle">Étudiant BTS SIO • Développeur Nuxt.js en Alternance</p>
      </div>

      <section class="about-section">
        <div class="about-card">
          <div class="card-icon">
            <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path>
              <circle cx="12" cy="7" r="4"></circle>
            </svg>
          </div>
          <h2 class="section-title">À propos</h2>
          <p>
            Bonjour et bienvenue sur mon Portfolio, je suis un étudiant en deuxième année de BTS SIO, en alternance.
          </p>
        </div>

        <div class="about-card">
          <div class="card-icon">
            <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <polyline points="16 18 22 12 16 6"></polyline>
              <polyline points="8 6 2 12 8 18"></polyline>
            </svg>
          </div>
          <h2 class="section-title">Ma passion</h2>
          <p>
            J'aime particulièrement travailler sur des interfaces modernes, propres et ergonomiques. J'accorde beaucoup 
            d'importance à la qualité du code, à l'optimisation et à l'expérience utilisateur.
          </p>
        </div>

        <div class="about-card">
          <div class="card-icon">
            <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path>
              <polyline points="22 4 12 14.01 9 11.01"></polyline>
            </svg>
          </div>
          <h2 class="section-title">Mes projets</h2>
          <p>
            Sur ce portfolio, vous trouverez mes différents projets, qu'ils soient réalisés en cours, en entreprise ou durant 
            mon temps libre. Mon objectif est de continuer à progresser, apprendre de nouvelles technologies et construire 
            des solutions utiles.
          </p>
        </div>
      </section>

      <div class="cta-section">
        <p class="cta-text">Naviguez à travers les différentes sections pour découvrir mon travail et mes compétences.</p>
        <div class="cta-buttons">
          <NuxtLink to="/projets" class="btn-primary">
            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M22 19a2 2 0 0 1-2 2H4a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h5l2 3h9a2 2 0 0 1 2 2z"></path>
            </svg>
            Voir mes projets
          </NuxtLink>
          <NuxtLink to="/contact" class="btn-secondary">
            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"></path>
            </svg>
            Me contacter
          </NuxtLink>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
definePageMeta({
  layout: "default",
});
</script>

<style lang="scss" scoped>
.home-page {
  min-height: 100vh;
  background: linear-gradient(135deg, #0d1117 0%, #161b22 100%);
  padding: 80px 20px 40px;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
}

.hero-section {
  text-align: center;
  margin-bottom: 80px;
  padding: 60px 20px;
}

.hero-title {
  display: flex;
  flex-direction: column;
  gap: 10px;
  margin-bottom: 20px;
}



.name {
  font-size: 4rem;
  font-weight: 700;
  background: linear-gradient(135deg, #58a6ff 0%, #79c0ff 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.hero-subtitle {
  font-size: 1.3rem;
  color: #8b949e;
  font-weight: 400;
}

.about-section {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 30px;
  margin-bottom: 60px;
}

.about-card {
  background: #161b22;
  border: 1px solid #30363d;
  border-radius: 12px;
  padding: 30px;
  transition: all 0.3s ease;
  
  &:hover {
    border-color: #58a6ff;
    box-shadow: 0 8px 30px rgba(88, 166, 255, 0.15);
  }
}

.card-icon {
  width: 50px;
  height: 50px;
  background: rgba(88, 166, 255, 0.1);
  border-radius: 10px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 20px;
  color: #58a6ff;
}

.section-title {
  font-size: 1.5rem;
  font-weight: 600;
  color: #c9d1d9;
  margin-bottom: 15px;
}

.about-card p {
  color: #8b949e;
  line-height: 1.7;
  font-size: 1rem;
  font-style: italic;
}

.cta-section {
  text-align: center;
  padding: 60px 20px;
  background: #161b22;
  border: 1px solid #30363d;
  border-radius: 12px;
  margin-top: 40px;
}

.cta-text {
  font-size: 1.2rem;
  color: #c9d1d9;
  margin-bottom: 30px;
  font-weight: 500;
}

.cta-buttons {
  display: flex;
  gap: 20px;
  justify-content: center;
  flex-wrap: wrap;
}

.btn-primary,
.btn-secondary {
  display: inline-flex;
  align-items: center;
  gap: 10px;
  padding: 14px 28px;
  border-radius: 8px;
  font-weight: 500;
  font-size: 1rem;
  text-decoration: none;
  transition: all 0.3s ease;
  
  svg {
    transition: transform 0.3s ease;
  }
  
  &:hover svg {
    transform: translateX(3px);
  }
}

.btn-primary {
  background: #238636;
  color: #fff;
  
  &:hover {
    background: #2ea043;
    box-shadow: 0 4px 20px rgba(35, 134, 54, 0.4);
  }
}

.btn-secondary {
  background: transparent;
  border: 1px solid #30363d;
  color: #c9d1d9;
  
  &:hover {
    border-color: #58a6ff;
    color: #58a6ff;
    box-shadow: 0 4px 20px rgba(88, 166, 255, 0.2);
  }
}

@media (max-width: 768px) {
  .hero-section {
    padding: 40px 10px;
    margin-bottom: 50px;
  }
  
  .name {
    font-size: 2.5rem;
  }
  
  .hero-subtitle {
    font-size: 1.1rem;
  }
  
  .about-section {
    grid-template-columns: 1fr;
  }
  
  .cta-buttons {
    flex-direction: column;
    align-items: stretch;
  }
  
  .btn-primary,
  .btn-secondary {
    width: 100%;
    justify-content: center;
  }
}
</style>