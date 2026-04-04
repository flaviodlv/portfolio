<template>
  <div class="home-page">
    <div class="container">
      <div class="hero-section">
        <h1 class="hero-title">
          <span class="name">Flavio DE OLIVEIRA</span>
          <span class="phone">06 09 01 56 07</span>
          <span class="mail">dolv.flavio@gmail.com</span>
        </h1>
        <p class="hero-subtitle">Étudiant BTS SIO • Développeur Informatique en Alternance</p>
      </div>

      <section class="about-section">
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
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
defineOptions({
  name: "HomePage",
});
</script>

<style lang="scss" scoped>
.home-page {
  min-height: 100vh;
  background: white;
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
  background: black;
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
  background: #ffffff;
  border: 1px solid #000000;
  border-radius: 12px;
  padding: 30px;
  transition: all 0.3s ease;

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
  color: #000000;
  margin-bottom: 15px;
}

.about-card p {
  color: #000000;
  line-height: 1.7;
  font-size: 1rem;
  font-style: italic;
}

.cta-section {
  text-align: center;
  padding: 60px 20px;
  background: #ffffff;
  border: 1px solid #000000;
  border-radius: 12px;
  margin-top: 40px;
}

.cta-text {
  font-size: 1.2rem;
  color: #000000;
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
    transition: transform 0.4s ease;
  }
}

.btn-primary {
  background: #238636;
  color: #fff;
  
  &:hover {
    background: #2ea043;
    box-shadow: 0 0px 10px rgba(17, 66, 27, 0.4);
  }
}

.btn-secondary {
  background: #238636;
  color: #fff;
  &:hover {
    background: #2ea043;
    box-shadow: 0 0px 10px rgba(17, 66, 27, 0.4);
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

  .mail {
    display: inline;
  }
}
</style>