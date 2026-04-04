<template>
    <div class="cv-page">
        <div class="container">
            <h1 class="page-title">CV</h1>
            <p class="page-subtitle">Découvrez mon parcours et mes compétences</p>
             <div class="cv-download">
                    <a href="\Flavio-De-Oliveira-FlowCV-Resume-20251115.pdf" target="_blank">
                        Lien vers le CV complet
                    </a>
                </div>
        </div>
    </div>
</template>

<script>
// eslint-disable-next-line no-undef
definePageMeta({
    layout: 'default'
})
</script>

<style lang="scss" scoped>

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
    background: rgb(0, 0, 0);
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

.cv-download {
    padding: 30px 40px;
    background: rgba(0, 0, 0, 0.1);
    text-align: center;
}

.cv-download a {
    color: #238636;
    font-size: 1.2rem;
    font-weight: 600;
    text-decoration: none;
    transition: color 0.3s ease;
    
    &:hover {
        color: #20c03d;
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