<template>
    <div class="veille-page">
        <div class="container">
            <h1 class="page-title">
                <a href="\veille.pdf" target="_blank">Veille Technologique</a>
            </h1>
            <p class="page-subtitle">
                Suivez mes découvertes et analyses des dernières tendances tech
            </p>

            <div class="featured-topic">
                <div class="topic-badge">
                    <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none"
                        stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                        <polygon
                            points="12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2">
                        </polygon>
                    </svg>
                    <span>Dernière découverte</span>
                </div>
                <h2 class="topic-title">DLSS - Deep Learning Super Sampling</h2>
                <p class="topic-intro">
                    Une technologie révolutionnaire de NVIDIA qui utilise l'intelligence
                    artificielle pour améliorer les performances graphiques dans les jeux
                    vidéo et applications 3D.
                </p>
            </div>

            <div class="content-grid">
                <div class="info-card main">
                    <div class="card-header">
                        <div class="icon-wrapper">
                            <svg xmlns="http://www.w3.org/2000/svg" width="28" height="28" viewBox="0 0 24 24"
                                fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"
                                stroke-linejoin="round">
                                <rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect>
                                <circle cx="8.5" cy="8.5" r="1.5"></circle>
                                <polyline points="21 15 16 10 5 21"></polyline>
                            </svg>
                        </div>
                        <h3>Qu'est-ce que le DLSS ?</h3>
                    </div>
                    <p>
                        Le <strong>DLSS (Deep Learning Super Sampling)</strong> est une
                        technologie d'upscaling basée sur l'IA développée par NVIDIA. Elle
                        utilise des réseaux de neurones pour générer des images en haute
                        résolution à partir d'images en résolution plus faible, offrant
                        ainsi des performances graphiques jusqu'à 2x supérieures tout en
                        maintenant une qualité visuelle exceptionnelle.
                    </p>
                    <p>
                        Contrairement aux techniques d'upscaling traditionnelles, le DLSS
                        analyse des milliers d'images de référence en ultra-haute qualité
                        pour "apprendre" à reconstruire intelligemment les détails
                        manquants, résultant en des images plus nettes et plus détaillées.
                    </p>
                </div>

                <div class="info-card">
                    <div class="card-header">
                        <div class="icon-wrapper">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"
                                fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"
                                stroke-linejoin="round">
                                <path d="M13 2L3 14h9l-1 8 10-12h-9l1-8z"></path>
                            </svg>
                        </div>
                        <h3>Avantages principaux</h3>
                    </div>
                    <ul class="benefits-list">
                        <li>
                            <span class="check-icon">✓</span>
                            <div>
                                <strong>Performances accrues :</strong> Jusqu'à 2x plus de FPS
                                sans compromettre la qualité visuelle
                            </div>
                        </li>
                        <li>
                            <span class="check-icon">✓</span>
                            <div>
                                <strong>Qualité supérieure :</strong> Images parfois plus nettes
                                que le rendu natif grâce à l'IA
                            </div>
                        </li>
                        <li>
                            <span class="check-icon">✓</span>
                            <div>
                                <strong>Ray Tracing optimisé :</strong> Permet d'activer le ray
                                tracing sans impacter les performances
                            </div>
                        </li>
                        <li>
                            <span class="check-icon">✓</span>
                            <div>
                                <strong>Efficacité énergétique :</strong> Moins de puissance
                                nécessaire pour un rendu haute qualité
                            </div>
                        </li>
                    </ul>
                </div>

                <div class="info-card">
                    <div class="card-header">
                        <div class="icon-wrapper">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"
                                fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"
                                stroke-linejoin="round">
                                <path d="M12 20h9"></path>
                                <path d="M16.5 3.5a2.12 2.12 0 0 1 3 3L7 19l-4 1 1-4L16.5 3.5z"></path>
                            </svg>
                        </div>
                        <h3>Comment ça fonctionne ?</h3>
                    </div>
                    <div class="process-steps">
                        <div class="step">
                            <div class="step-number">1</div>
                            <p>
                                Le jeu est rendu à une résolution inférieure (ex: 1080p au lieu
                                de 4K)
                            </p>
                        </div>
                        <div class="step">
                            <div class="step-number">2</div>
                            <p>
                                Le modèle d'IA analyse l'image, les vecteurs de mouvement et les
                                informations de profondeur
                            </p>
                        </div>
                        <div class="step">
                            <div class="step-number">3</div>
                            <p>
                                L'IA reconstruit intelligemment les détails pour générer une
                                image en haute résolution
                            </p>
                        </div>
                        <div class="step">
                            <div class="step-number">4</div>
                            <p>
                                L'image finale est affichée avec une qualité proche ou
                                supérieure au rendu natif
                            </p>
                        </div>
                    </div>
                </div>

                <div class="info-card">
                    <div class="card-header">
                        <div class="icon-wrapper">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"
                                fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"
                                stroke-linejoin="round">
                                <polyline points="22 12 18 12 15 21 9 3 6 12 2 12"></polyline>
                            </svg>
                        </div>
                        <h3>Évolution du DLSS</h3>
                    </div>
                    <div class="versions">
                        <div class="version-item">
                            <strong>DLSS 1.0</strong>
                            <p>Première version, qualité variable selon les jeux</p>
                        </div>
                        <div class="version-item">
                            <strong>DLSS 2.0</strong>
                            <p>Amélioration majeure, qualité constante et universelle</p>
                        </div>
                        <div class="version-item">
                            <strong>DLSS 3.0</strong>
                            <p>Génération d'images entières par IA (Frame Generation)</p>
                        </div>
                        <div class="version-item current">
                            <strong>DLSS 3.5</strong>
                            <p>
                                Ajout du Ray Reconstruction pour un éclairage encore plus
                                réaliste
                            </p>
                        </div>
                    </div>
                </div>
            </div>

            <div class="tech-impact-card">
                <div class="card-header">
                    <div class="icon-wrapper primary">
                        <svg xmlns="http://www.w3.org/2000/svg" width="28" height="28" viewBox="0 0 24 24" fill="none"
                            stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                            <path
                                d="M21 16V8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16z">
                            </path>
                            <polyline points="3.27 6.96 12 12.01 20.73 6.96"></polyline>
                            <line x1="12" y1="22.08" x2="12" y2="12"></line>
                        </svg>
                    </div>
                    <h3>Impact sur l'industrie du jeu vidéo</h3>
                </div>
                <p>
                    Le DLSS représente un tournant majeur dans l'industrie du gaming. En
                    permettant des performances élevées avec des graphismes de qualité
                    supérieure, il rend le ray tracing et les résolutions 4K/8K
                    accessibles à un plus large public. Cette technologie influence
                    également le développement des jeux, les studios pouvant désormais
                    créer des environnements plus détaillés sans sacrifier les
                    performances.
                </p>
                <p>
                    Au-delà du gaming, le DLSS trouve des applications dans la création de
                    contenu 3D, le streaming, et pourrait inspirer des innovations
                    similaires dans d'autres domaines utilisant l'IA pour l'optimisation
                    en temps réel.
                </p>
            </div>
        </div>
    </div>
</template>

<script>
definePageMeta({
    layouts: "default",
});
</script>

<style lang="scss" scoped>
.veille-page {
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
    margin-bottom: 20px;
}

.featured-topic {
    background: linear-gradient(135deg,
            rgba(88, 166, 255, 0.1) 0%,
            rgba(88, 166, 255, 0.05) 100%);
    border: 2px solid #58a6ff;
    border-radius: 16px;
    padding: 40px;
    margin-bottom: 40px;
    text-align: center;
}

.topic-badge {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    padding: 8px 16px;
    background: rgba(255, 215, 0, 0.1);
    border: 1px solid #ffd700;
    border-radius: 20px;
    color: #ffd700;
    font-size: 0.9rem;
    font-weight: 500;
    margin-bottom: 20px;
}

.topic-title {
    font-size: 2.5rem;
    font-weight: 700;
    color: #c9d1d9;
    margin-bottom: 15px;
}

.topic-intro {
    font-size: 1.2rem;
    color: #8b949e;
    max-width: 800px;
    margin: 0 auto;
    line-height: 1.7;
}

.content-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: 30px;
    margin-bottom: 40px;
}

.info-card {
    background: #161b22;
    border: 1px solid #30363d;
    border-radius: 12px;
    padding: 30px;
    transition: all 0.3s ease;

    &.main {
        grid-column: 1 / -1;
    }
}

.card-header {
    display: flex;
    align-items: center;
    gap: 15px;
    margin-bottom: 20px;

    h3 {
        color: #c9d1d9;
        font-size: 1.4rem;
        font-weight: 600;
        margin: 0;
    }
}

.icon-wrapper {
    width: 50px;
    height: 50px;
    background: rgba(88, 166, 255, 0.1);
    border: 1px solid #58a6ff;
    border-radius: 10px;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #58a6ff;
    flex-shrink: 0;

    &.primary {
        background: rgba(88, 166, 255, 0.2);
    }
}

.info-card p {
    color: #8b949e;
    line-height: 1.8;
    font-size: 1.05rem;
    margin-bottom: 15px;

    strong {
        color: #c9d1d9;
        font-weight: 600;
    }

    &:last-child {
        margin-bottom: 0;
    }
}

.benefits-list {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    flex-direction: column;
    gap: 15px;

    li {
        display: flex;
        gap: 12px;
        align-items: start;
        color: #8b949e;
        line-height: 1.6;
    }
}

.check-icon {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 24px;
    height: 24px;
    background: rgba(35, 134, 54, 0.2);
    border-radius: 50%;
    color: #2ea043;
    font-weight: bold;
    flex-shrink: 0;
    margin-top: 2px;
}

.process-steps {
    display: flex;
    flex-direction: column;
    gap: 15px;
}

.step {
    display: flex;
    gap: 15px;
    align-items: start;

    p {
        margin: 0;
        color: #8b949e;
        line-height: 1.6;
    }
}

.step-number {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 32px;
    height: 32px;
    background: rgba(88, 166, 255, 0.2);
    border: 2px solid #58a6ff;
    border-radius: 50%;
    color: #58a6ff;
    font-weight: 700;
    flex-shrink: 0;
}

.versions {
    display: flex;
    flex-direction: column;
    gap: 15px;
}

.version-item {
    padding: 15px;
    background: rgba(88, 166, 255, 0.05);
    border-left: 3px solid #30363d;
    border-radius: 6px;
    transition: all 0.3s ease;

    strong {
        display: block;
        color: #c9d1d9;
        font-size: 1.1rem;
        margin-bottom: 5px;
    }

    p {
        margin: 0;
        color: #8b949e;
        font-size: 0.95rem;
    }

    &.current {
        border-left-color: #58a6ff;
        background: rgba(88, 166, 255, 0.1);

        strong {
            color: #58a6ff;
        }
    }
}

.tech-impact-card {
    background: #161b22;
    border: 1px solid #30363d;
    border-radius: 12px;
    padding: 32px;
    margin-bottom: 40px;
    transition: all 0.3s ease;
}

.tech-impact-card p {
    color: #ffffff;
    line-height: 1.8;
    margin-bottom: 15px;
}

.cta-section {
    text-align: center;
    padding: 40px 20px;
    background: #161b22;
    border: 1px solid #30363d;
    border-radius: 12px;
}

.cta-text {
    font-size: 1.2rem;
    color: #c9d1d9;
    margin-bottom: 25px;
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
    .page-title {
        font-size: 2rem;
    }

    .featured-topic {
        padding: 30px 20px;
    }

    .topic-title {
        font-size: 1.8rem;
    }

    .content-grid {
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
