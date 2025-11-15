<template>
    <div class="cv-page">
        <div class="container">
            <h1 class="page-title">Curriculum Vitae</h1>
            <p class="page-subtitle">Découvrez mon parcours et mes compétences</p>

            <div class="cv-card">
                <div class="cv-header">
                    <div class="profile-section">
                        <div class="profile-icon">
                            <svg xmlns="http://www.w3.org/2000/svg" width="64" height="64" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path>
                                <circle cx="12" cy="7" r="4"></circle>
                            </svg>
                        </div>
                        <div class="profile-info">
                            <h2>Flavio De Oliveira</h2>
                            <p class="role">Étudiant en Informatique • BTS SIO SLAM</p>
                            <p class="description">
                                Passionné par le développement web moderne et l'intelligence artificielle, 
                                je suis actuellement en alternance et je souhaite approfondir mes compétences 
                                en développement full-stack et IA.
                            </p>
                        </div>
                    </div>
                </div>

                <div class="cv-content">
                    <div class="info-grid">
                        <div class="info-item">
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path>
                                <polyline points="22,6 12,13 2,6"></polyline>
                            </svg>
                            <span>dolv.flavio@gmail.com</span>
                        </div>
                        <div class="info-item">
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"></path>
                                <circle cx="12" cy="10" r="3"></circle>
                            </svg>
                            <span>Paris, France</span>
                        </div>
                        <div class="info-item">
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <rect x="2" y="7" width="20" height="14" rx="2" ry="2"></rect>
                                <path d="M16 21V5a2 2 0 0 0-2-2h-4a2 2 0 0 0-2 2v16"></path>
                            </svg>
                            <span>23 ans</span>
                        </div>
                        <div class="info-item">
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"></path>
                                <rect x="2" y="9" width="4" height="12"></rect>
                                <circle cx="4" cy="4" r="2"></circle>
                            </svg>
                            <a href="https://linkedin.com/in/flvdlv" target="_blank" rel="noopener noreferrer">linkedin.com/in/flvdlv</a>
                        </div>
                    </div>

                    <div class="highlights-section">
                        <div class="highlight-card">
                            <div class="highlight-icon">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                    <path d="M22 10v6M2 10l10-5 10 5-10 5z"></path>
                                    <path d="M6 12v5c3 3 9 3 12 0v-5"></path>
                                </svg>
                            </div>
                            <h3>Formation</h3>
                            <p>BTS SIO SLAM en alternance</p>
                            <p class="sub">Aurlom BTS+ • 2024-2026</p>
                        </div>

                        <div class="highlight-card">
                            <div class="highlight-icon">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                    <polyline points="16 18 22 12 16 6"></polyline>
                                    <polyline points="8 6 2 12 8 18"></polyline>
                                </svg>
                            </div>
                            <h3>Compétences</h3>
                            <p>JavaScript, Python, Vue.js</p>
                            <p class="sub">HTML, CSS, Nuxt.js, IA</p>
                        </div>

                        <div class="highlight-card">
                            <div class="highlight-icon">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                    <path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"></path>
                                    <polyline points="7 10 12 15 17 10"></polyline>
                                    <line x1="12" y1="15" x2="12" y2="3"></line>
                                </svg>
                            </div>
                            <h3>Langues</h3>
                            <p>Français (Maternel)</p>
                            <p class="sub">Anglais (Fluent) • Portugais</p>
                        </div>
                    </div>
                </div>

                <div class="cv-download">
                    <a href="/" download class="btn-download">
                        CV complet 
                    </a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
definePageMeta({
    layout: 'default'
})
</script>

<style lang="scss" scoped>
.cv-page {
    min-height: 100vh;
    background: linear-gradient(135deg, #0d1117 0%, #161b22 100%);
    padding: 80px 20px 40px;
}

.container {
    max-width: 1000px;
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

.cv-card {
    background: #161b22;
    border: 1px solid #30363d;
    border-radius: 16px;
    overflow: hidden;
    box-shadow: 0 8px 30px rgba(0, 0, 0, 0.3);
}

.cv-header {
    background: linear-gradient(135deg, rgba(88, 166, 255, 0.1) 0%, rgba(88, 166, 255, 0.05) 100%);
    border-bottom: 1px solid #30363d;
    padding: 40px;
}

.profile-section {
    display: flex;
    gap: 30px;
    align-items: start;
}

.profile-icon {
    width: 100px;
    height: 100px;
    background: rgba(88, 166, 255, 0.1);
    border: 2px solid #58a6ff;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #58a6ff;
    flex-shrink: 0;
}

.profile-info {
    flex: 1;
    
    h2 {
        font-size: 2.2rem;
        font-weight: 700;
        color: #c9d1d9;
        margin: 0 0 10px 0;
    }
    
    .role {
        font-size: 1.2rem;
        color: #58a6ff;
        margin-bottom: 15px;
        font-weight: 500;
    }
    
    .description {
        color: #8b949e;
        line-height: 1.7;
        font-size: 1rem;
    }
}

.cv-content {
    padding: 40px;
}

.info-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
    margin-bottom: 40px;
}

.info-item {
    display: flex;
    align-items: center;
    gap: 12px;
    color: #8b949e;
    font-size: 0.95rem;
    
    svg {
        color: #58a6ff;
        flex-shrink: 0;
    }
    
    a {
        color: #58a6ff;
        text-decoration: none;
        transition: color 0.2s ease;
        
        &:hover {
            color: #79c0ff;
            text-decoration: underline;
        }
    }
}

.highlights-section {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
}

.highlight-card {
    background: rgba(88, 166, 255, 0.05);
    border: 1px solid #30363d;
    border-radius: 12px;
    padding: 24px;
    transition: all 0.3s ease;
}

.highlight-icon {
    width: 50px;
    height: 50px;
    background: rgba(88, 166, 255, 0.1);
    border-radius: 10px;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #58a6ff;
    margin-bottom: 15px;
}

.highlight-card h3 {
    font-size: 1.2rem;
    font-weight: 600;
    color: #c9d1d9;
    margin: 0 0 10px 0;
}

.highlight-card p {
    color: #8b949e;
    font-size: 0.95rem;
    margin: 5px 0;
    
    &.sub {
        font-size: 0.85rem;
        color: #6e7681;
    }
}

.cv-download {
    padding: 30px 40px;
    background: rgba(35, 134, 54, 0.05);
    border-top: 1px solid #30363d;
    text-align: center;
}

.btn-download {
    display: inline-flex;
    align-items: center;
    gap: 12px;
    padding: 16px 32px;
    background: #238636;
    color: #fff;
    text-decoration: none;
    border-radius: 8px;
    font-weight: 500;
    font-size: 1.1rem;
    transition: all 0.3s ease;
    
    svg {
        transition: transform 0.3s ease;
    }
    
    &:hover svg {
        transform: translateY(3px);
    }
}

@media (max-width: 768px) {
    .page-title {
        font-size: 2rem;
    }
    
    .cv-header {
        padding: 30px 20px;
    }
    
    .profile-section {
        flex-direction: column;
        align-items: center;
        text-align: center;
    }
    
    .profile-icon {
        width: 80px;
        height: 80px;
        
        svg {
            width: 48px;
            height: 48px;
        }
    }
    
    .profile-info h2 {
        font-size: 1.8rem;
    }
    
    .cv-content {
        padding: 30px 20px;
    }
    
    .info-grid,
    .highlights-section {
        grid-template-columns: 1fr;
    }
    
    .cv-download {
        padding: 25px 20px;
    }
    
    .btn-download {
        width: 100%;
        justify-content: center;
    }
}
</style>