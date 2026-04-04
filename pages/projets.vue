<template>
    <div class="projects-page">
        <div class="container">
            <h1 class="page-title">Mes Projets</h1>
            <p class="page-subtitle">Découvrez mes réalisations et expérimentations</p>
            <h1>Projets scolaire</h1>
             <div class="project-card">
                    <div class="project-header">
                        <h2 class="project-title">PPE 1 : Réalisation d’un site Web de e-commerce</h2>
                    </div>
                    <p class="project-description">
                        Projet Professionnel Encadré réalisé en première année dans le cadre de ma formation.
                    </p>
                    <div class="project-links">
                        <a target="_blank" href="https://drive.google.com/drive/folders/1H8juEu5YwMbv43fnoOrz8SF_Hb0wnFGV" class="btn-link">Voir la documentation</a>
                        
                    </div>
                </div>
                <div class="project-card">
                    <div class="project-header">
                        <h2 class="project-title">PPE 2 : Application Windows permettant de créer des interventions sur des produits</h2>
                    </div>
                    <p class="project-description">
                        Projet Professionnel Encadré réalisé en deuxième année dans le cadre de ma formation.
                    </p>
                    <div class="project-links">
                        <a target="_blank" href="https://drive.google.com/drive/folders/1qDKq8KDi-vJNLCOoh4nnSDBB5a77C_tP" class="btn-link">Voir la documentation</a>
                    </div>
                </div>
                <hr>
                <h1>Projets extra-scolaire</h1>
            <div class="projects-grid">
                <div class="project-card">
                    <div class="project-header">
                        <h2 class="project-title">Collection de projets réalisés en extra-scolaire</h2>
                    </div>
                    <div class="project-links">
                        <a href="https://github.com/flaviodlv/" target="_blank" class="btn-link">Voir les projets</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
// eslint-disable-next-line no-undef
definePageMeta({
    layouts: 'default'
})
</script>

<style lang="scss" scoped>
.projects-page {
    min-height: 100vh;
    background: white;
    padding: 80px 20px 40px;
}

.container {
    max-width: 1200px;
    margin: 0 auto;
}

.page-title {
    font-size: 3rem;
    font-weight: 700;
    color: #fff;
    text-align: center;
    margin-bottom: 10px;
    background: black;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}

.page-subtitle {
    text-align: center;
    color: #8b949e;
    font-size: 1.1rem;
    margin-bottom: 60px;
}

.projects-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
    gap: 30px;
}

.project-card {
    background: #ffffff;
    border: 1px solid #000000;
    border-radius: 12px;
    padding: 24px;
    transition: all 0.3s ease;
}

.project-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 16px;
}

.project-title {
    font-size: 1.5rem;
    font-weight: 600;
    color: #000000;
    margin: 0;
}


.project-description {
    color: #000000;
    line-height: 1.6;
    margin-bottom: 20px;
    min-height: 60px;
}

.project-links {
    display: flex;
    gap: 12px;
}

.btn-link {
    flex: 1;
    padding: 10px 20px;
    background: #238636;
    color: #fff;
    text-decoration: none;
    border-radius: 6px;
    text-align: center;
    font-weight: 500;
    transition: all 0.2s ease;
    
    &:hover {
        background: #2ea043;
    }
}

@media (max-width: 768px) {
    .page-title {
        font-size: 2rem;
    }
    
    .projects-grid {
        grid-template-columns: 1fr;
    }
    
    .projects-page {
        padding: 60px 15px 30px;
    }
}
</style>