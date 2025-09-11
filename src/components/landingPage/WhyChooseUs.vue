<template>
  <section id="why-choose-us" class="why-choose-us py-5">
    <div class="container">
        <div class="row align-items-center">
            <div class="col-12 col-lg-8 order-lg-1 order-2">
                <h2>Pourquoi choisir Visale ?</h2>
                <ul>
                  <li>Garantie 100 % gratuite pour les propriétaires particuliers</li>
                  <li>Jusqu'à 36 mois de loyers impayés pris en charge (9 mois en parc social)</li>
                  <li>Jusqu'à 2 mois de dégradations locatives remboursés</li>
                  <li>Aucune franchise, aucun délai de carence</li>
                  <li>100 % digital : gérez tout en quelques clics</li>
                  <li>Accompagnement Action Logement en cas d'impayé et indemnisation rapide</li>
                </ul>
            </div>
            
            <div class="col-12 col-lg-4 text-center order-lg-2 order-1 mb-4 mb-lg-0">
                <div class="why-choose-us-img">
                  <img src="/img/landing-page/why-choose-us.svg" alt="Feature visale" height="430" class="me-2">
                </div>
            </div>
            
        </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'WhyChooseUs',
}
</script>

<style scoped>
  .why-choose-us {
    overflow: hidden;
  }

  .why-choose-us h2{
      color: #193B68;
      font-size: 40px;
      font-style: normal;
      font-weight: 600;
      margin-bottom: 40px;
  }

  .why-choose-us ul{
      list-style: disc;
  }

  .why-choose-us ul li{
      color: #000;
      font-size: 18px;
      font-style: normal;
      font-weight: 500;
      line-height: 38px;
  }

  .why-choose-us-img{
      max-height: 332px;
  }

  @media (max-width: 992px) {
  .why-choose-us-img {
    overflow: visible;
  }

  .why-choose-us-img img{
    max-width: 100%;
  }
}
</style>
