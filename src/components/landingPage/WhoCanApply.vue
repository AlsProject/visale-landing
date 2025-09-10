<template>
  <section id="who-can-apply" class="who-can-apply py-5">
    <div class="container">
        <h2>A quels locataires s’adresse Visale ?</h2>
        <div class="row">
            <div class="col-12 col-lg-3 d-flex flex-column justify-content-start align-items-center mb-3 mb-lg-0">
              <div class="who-can-apply-img">
                <div class="circle"></div>
                <img src="/img/landing-page/alternant-homme.svg" alt="Alternant visale"  class="me-2 alternant-homme">
              </div>
              <div class="text-center">
                <h3>Moins de 31 ans</h3>
                <p><strong>Étudiants, alternants, jeunes actifs</strong>, quelle que soit leur situation.</p>
              </div>
            </div>
            <div class="col-12 col-lg-3 d-flex flex-column justify-content-start align-items-center mb-3 mb-lg-0">
              <div class="who-can-apply-img">
                <div class="circle"></div>
                <img src="/img/landing-page/salarie-femme.svg" alt="Salarié visale"  class="me-2 salarie-femme">
              </div>
              <div class="text-center">
                <h3>Plus de 31 ans</h3>
                <p><strong>Salariés du privé avec revenu ≤ 1 500 €/mois</strong> ou en mobilité (CDD, période d'essai, mutation).</p>
              </div>
            </div>
            <div class="col-12 col-lg-3 d-flex flex-column justify-content-start align-items-center mb-3 mb-lg-0">
              <div class="who-can-apply-img">
                <div class="circle"></div>
                <img src="/img/landing-page/locataire-femme.svg" alt="Salarié visale"  class="me-2 locataire-femme">
              </div>
              <div class="text-center">
                <h3>Bail mobilité</h3>
                <p><strong>Locataires de tout âge en contrat court</strong> (mission, stage, formation) dans un logement meublé.</p>
              </div>
            </div>
            <div class="col-12 col-lg-3 d-flex flex-column justify-content-start align-items-center mb-3 mb-lg-0">
              <div class="who-can-apply-img">
                <div class="circle"></div>
                <img src="/img/landing-page/saisonnier-homme.svg" alt="Salarié visale"  class="me-2 saisonnier-homme">
              </div>
              <div class="text-center">
                <h3>Saisonniers</h3>
                <p><strong>18 ans minimum, contrat de travail avec la mention «saisonnier»</strong> loyer maximum 600 € (800€ en Ile de France).</p>
              </div>
            </div>
        </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'WhoCanApply',
}
</script>

<style scoped>
  .who-can-apply{
    background-color: #ECECEC;
  }

  .who-can-apply h2{
    color: #193B68;
    font-size: 40px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 80px;
  }

  .who-can-apply h3{
    color: #E6224B;
    font-size: 20px;
    font-style: normal;
    font-weight: 600;
    line-height: 60px;
  }

  .who-can-apply p{
    color: #000;
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
  }

  .who-can-apply-img{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 200px;
    height: 150px;
    margin: 0 auto;
    position: relative;
  }

  .circle{
    width: 80px;
    height: 80px;
    border-radius: 50%;
    background-color: #009EE3;
    position: absolute;
  }

  .who-can-apply-img img {
    object-fit: contain;
    z-index: 2;
    position: absolute;
    top: 40%;
    left: 52%;
    transform: translate(-50%, -50%);
  }

  .who-can-apply-img .alternant-homme{
    top:36%;
    left: 58%;
  }   

  .who-can-apply-img .salarie-femme{
    left: 50%;
  }
</style>
