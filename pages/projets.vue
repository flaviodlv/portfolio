<template>
    <div class="projects-page">
        <div class="container">
            <h1 class="page-title">Mes Projets</h1>
            <p class="page-subtitle">Découvrez mes réalisations et expérimentations</p>

            <div class="projects-grid">
                <div class="project-card">
                    <div class="project-header">
                        <h2 class="project-title">mini-nuxt-project</h2>
                        <span class="badge">Public</span>
                    </div>
                    <div class="project-tech">
                        <span class="tech-badge vue">
                            <span class="tech-dot"></span>
                            Vue
                        </span>
                    </div>
                    <p class="project-description">
                        Un projet minimaliste utilisant Nuxt.js pour explorer les fonctionnalités du framework.
                    </p>
                    <div class="project-links">
                        <a href="#" class="btn-link">Voir le code</a>
                        <a href="#" class="btn-link secondary">Demo</a>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-header">
                        <h2 class="project-title">pygame</h2>
                        <span class="badge">Public</span>
                    </div>
                    <div class="project-tech">
                        <span class="tech-badge python">
                            <span class="tech-dot"></span>
                            Python
                        </span>
                    </div>
                    <p class="project-description">
                        Collection de jeux développés avec Pygame pour apprendre le développement de jeux 2D.
                    </p>
                    <div class="project-links">
                        <a href="#" class="btn-link">Voir le code</a>
                        <a href="#" class="btn-link secondary">Demo</a>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-header">
                        <h2 class="project-title">Miningame</h2>
                        <span class="badge">Public</span>
                    </div>
                    <div class="project-tech">
                        <span class="tech-badge python">
                            <span class="tech-dot"></span>
                            Python
                        </span>
                    </div>
                    <p class="project-description">
                        Jeu PyGame 2D de mineur - Explorez, minez et survivez dans un monde souterrain généré procéduralement.
                    </p>
                    <div class="project-links">
                        <a href="#" class="btn-link">Voir le code</a>
                        <a href="#" class="btn-link secondary">Demo</a>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-header">
                        <h2 class="project-title">portfolio</h2>
                        <span class="badge">Public</span>
                    </div>
                    <div class="project-tech">
                        <span class="tech-badge vue">
                            <span class="tech-dot"></span>
                            Vue
                        </span>
                    </div>
                    <p class="project-description">
                        Ce portfolio que vous consultez actuellement, développé avec Nuxt.js et Vue 3.
                    </p>
                    <div class="project-links">
                        <a target="_blank" href="https://github.com/flaviodlv/portfolio" class="btn-link">Voir le code</a>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-header">
                        <h2 class="project-title">PPE</h2>
                        <span class="badge">Public</span>
                    </div>
                    <div class="project-tech">
                        <span class="tech-badge vue">
                            <span class="tech-dot"></span>
                            Vue
                        </span>
                    </div>
                    <p class="project-description">
                        Projet Professionnel Encadré réalisé dans le cadre de ma formation BTS SIO.
                    </p>
                    <div class="project-links">
                        <a target="_blank" href="https://github.com/flaviodlv/ppe" class="btn-link">Voir le code</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
definePageMeta({
    layouts: 'default'
})
</script>

<style lang="scss" scoped>
.projects-page {
    min-height: 100vh;
    background: linear-gradient(135deg, #0d1117 0%, #161b22 100%);
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
    background: linear-gradient(135deg, #58a6ff 0%, #79c0ff 100%);
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
    background: #161b22;
    border: 1px solid #30363d;
    border-radius: 12px;
    padding: 24px;
    transition: all 0.3s ease;
    
    &:hover {
        transform: translateY(-5px);
        border-color: #58a6ff;
        box-shadow: 0 8px 30px rgba(88, 166, 255, 0.15);
    }
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
    color: #58a6ff;
    margin: 0;
}

.badge {
    padding: 4px 12px;
    background: rgba(88, 166, 255, 0.1);
    border: 1px solid #58a6ff;
    border-radius: 20px;
    font-size: 0.75rem;
    color: #58a6ff;
    font-weight: 500;
}

.project-tech {
    display: flex;
    gap: 10px;
    margin-bottom: 16px;
}

.tech-badge {
    display: flex;
    align-items: center;
    gap: 6px;
    padding: 4px 12px;
    background: rgba(139, 148, 158, 0.1);
    border-radius: 16px;
    font-size: 0.85rem;
    color: #8b949e;
    
    &.vue {
        .tech-dot {
            background: #42b883;
        }
    }
    
    &.python {
        .tech-dot {
            background: #3776ab;
        }
    }
}

.tech-dot {
    width: 10px;
    height: 10px;
    border-radius: 50%;
}

.project-description {
    color: #c9d1d9;
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
    
    &.secondary {
        background: transparent;
        border: 1px solid #30363d;
        color: #c9d1d9;
        
        &:hover {
            border-color: #58a6ff;
            color: #58a6ff;
        }
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