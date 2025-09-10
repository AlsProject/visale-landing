<template>
  <section id="accueil" class="hero py-5" style="margin-top: 76px;">
    <div class="container">
      <div class="d-flex align-items-center justify-content-center flex-lg-nowrap flex-wrap gap-4">
          <div class="persona-bailleur">
              <img src="/img/landing-page/persona-bailleurs.svg" alt="Persona Bailleurs" class="me-2 float-levitation">
          </div>
          <div class="hero-title text-center">
              <h1>Louez en toute confiance, Visale s'occupe du reste.</h1>
              <h2>Protégez vos loyers gratuitement jusqu'à 36 mois. Visale, la garantie simple et fiable des propriétaires.</h2>
          </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Hero'
}
</script>

<style scoped>
  .hero {
    min-height: 300px;
    background: linear-gradient(90deg,  #193B68 0%,  #009EE3 100%);
  }


  .hero-title h1{
    color: #FFF;
    font-size: 40px;
    font-style: normal;
    font-weight: 700;
    line-height: 40px; /* 125% */
  }

  .hero-title h2{
    color: #FFF;
    font-size: 20px;
    font-style: normal;
    font-weight: 500;
    line-height: 40px; /* 125% */
  }

  .float-levitation {
  animation: levitation 3s ease-in-out infinite;
}

@keyframes levitation {
  0%, 100% { 
    transform: translateY(0px); 
  }
  50% { 
    transform: translateY(-15px); 
  }
}


</style>
