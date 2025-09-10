<template>
  <section id="clients-trust" class="clients-trust pt-5">
    <div class="container">
        <h2>Ils nous font confiance</h2>
        <div class="row">
            <div class="col-12 col-lg-6">
                <div class="capture-video position-relative" data-bs-toggle="modal" data-bs-target="#videoModal">
                    <img src="/img/landing-page/capture-video.webp" alt="Video">
                    <!-- Icône YouTube transparente -->
                    <div class="youtube-overlay position-absolute top-50 start-50 translate-middle">
                        <i class="fab fa-youtube youtube-icon"></i>
                    </div>
                </div>
            </div>
            <div class="col-12 col-lg-6">
                <div class="testimonial">
                    <h3>Témoignages</h3>
                    <p><i>“C'est gagnant pour le locataire qui trouve beaucoup plus facilement, et pour le propriétaire qui a une garantie extrêmement solide.”</i></p>
                    <p><i>“Ça rassure les bailleurs, et on est sûrs de pouvoir toucher nos loyers en cas d'impayés.”</i></p>
                    <span><i>Témoignage vidéo, bailleur utilisateur de Visale</i></span>
                </div>
            </div>
        </div>

        <div class="d-flex align-items-end justify-content-center flex-lg-nowrap flex-wrap gap-4 pt-5">
            <div>
                <img src="/img/landing-page/satisfaction.svg" alt="Satisfaction">
            </div>
            <div class="satisfaction-text d-flex flex-column justify-content-start align-items-center text-center py-5">
                <h3>90 % des bailleurs sont satisfaits de Visale.<br>Pourquoi pas vous ?</h3>
                <p>Inscrivez-vous gratuitement et découvrez comment Visale peut sécuriser vos revenus tout en facilitant l’accès au logement.</p>
                <div class="d-flex align-items-center justify-content-center flex-lg-nowrap ere le gitignor deja 
                flex-wrap gap-4">
                    <a class="btn btn-secondary mb-3 mb-lg-0" href="">En savoir plus sur Visale</a>
                    <a class="btn btn-primary mb-3 mb-lg-0" href="">Je crée mon compte bailleur</a>
                </div>
                
            </div>
        </div>
    </div>

    <!-- Modal Vidéo -->
    <div class="modal fade" id="videoModal" tabindex="-1" aria-labelledby="videoModalLabel" aria-hidden="true" data-bs-backdrop="static" data-bs-keyboard="false">
      <div class="modal-dialog modal-lg modal-dialog-centered">
        <div class="modal-content">
          <div class="modal-header">
            <h5 class="modal-title" id="videoModalLabel">Témoignage Visale</h5>
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
          </div>
          <div class="modal-body p-0">
            <div class="ratio ratio-16x9">
              <iframe 
                id="youtubeVideo"
                src=""
                title="YouTube video player" 
                frameborder="0" 
                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" 
                allowfullscreen>
              </iframe>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'ClientsTrust',
  mounted() {
    // Gestion de l'ouverture de la modal
    const videoModal = document.getElementById('videoModal');
    const youtubeVideo = document.getElementById('youtubeVideo');
    
    // URL de la vidéo YouTube avec autoplay et start time
    const videoUrl = 'https://www.youtube.com/embed/HiGwIfYo2Vo?autoplay=1&start=5&rel=0&modestbranding=1';
    
    // Quand la modal s'ouvre
    videoModal.addEventListener('shown.bs.modal', () => {
      youtubeVideo.src = videoUrl;
    });
    
    // Quand la modal se ferme
    videoModal.addEventListener('hidden.bs.modal', () => {
      youtubeVideo.src = '';
    });
  }
}
</script>

<style scoped>
.clients-trust {
  background-color: #fff;
}

.clients-trust h2 {
  color: #193B68;
  font-size: 40px;
  font-weight: 600;
  margin-bottom: 80px;
}

.testimonial h3 {
  color: #193B68;
  font-size: 20px;
  font-weight: 600;
  margin-bottom: 40px;
}

.testimonial p{
    font-size: 18px;
    font-weight: normal;
    margin-bottom: 40px;
}

.testimonial span{
    font-size: 14px;
    font-weight: normal;
    margin-bottom: 40px;
}

.capture-video {
    cursor: pointer;
    border-radius: 8px;
    overflow: hidden;
    transition: transform 0.2s ease;
}

.capture-video:hover {
    transform: scale(1.02);
}

.capture-video img{
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.youtube-overlay {
    z-index: 2;
    pointer-events: none;
}

.youtube-icon {
    font-size: 4rem;
    color: rgba(255, 255, 255, 0.8);
    text-shadow: 0 2px 10px rgba(0, 0, 0, 0.5);
    transition: all 0.3s ease;
}

.capture-video:hover .youtube-icon {
    color: rgba(255, 255, 255, 1);
    transform: scale(1.1);
}

/* Responsive */
@media (max-width: 768px) {
    .youtube-icon {
        font-size: 3rem;
    }
}

/* Modal Video Styles */
.modal-backdrop {
    background-color: rgba(0, 0, 0, 0.85) !important;
}

.modal-content {
    border: 16px solid rgba(255, 255, 255, 0.2);
    border-radius: 16px;
    overflow: hidden;
    box-shadow: 
        0 25px 50px rgba(0, 0, 0, 0.4),
        0 0 0 1px rgba(255, 255, 255, 0.1),
        inset 0 1px 0 rgba(255, 255, 255, 0.2);
    background: rgba(255, 255, 255, 0.9);
}

.modal-header {
    background: linear-gradient(135deg, rgba(25, 59, 104, 0.9), rgba(0, 158, 227, 0.8));
    color: white;
    border-bottom: 1px solid rgba(255, 255, 255, 0.1);
    position: relative;
}

.modal-header::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: rgba(255, 255, 255, 0.05);
    pointer-events: none;
}

.modal-title {
    font-weight: 600;
}

.btn-close {
    filter: invert(1);
    opacity: 0.8;
    transition: opacity 0.2s ease;
}

.btn-close:hover {
    opacity: 1;
}

.ratio iframe {
    border-radius: 0 0 12px 12px;
}

.satisfaction-text h3 {
    color: #193B68;
    font-size: 40px;
    font-weight: 600;
    margin-bottom: 40px;
}

.satisfaction-text p {
    font-size: 18px;
    color: #000;
    font-weight: normal;
    margin-bottom: 40px;
}

.btn{
    border-radius: 30px;
}

.btn-primary{
    background-color: #E6224B;
    color: #fff;
    border: 1px solid #E6224B;
}

.btn-primary:hover{
    background-color: transparent;
    color: #E6224B;
    font-weight: 600;
}

.btn-secondary{
    background-color: #193B68;
    color: #fff;
    border: 1px solid #193B68;
}

.btn-secondary:hover{
    background-color: transparent;
    color: #193B68;
    font-weight: 600;
}
</style>
