<template>
  <section id="workflow" class="workflow py-5">
    <div class="container">
      
    <h2>Comment ça fonctionne ?</h2>
       
      
      <div class="row justify-content-center">
        <!-- Étape 1 -->
        <div class="workflow-step col-12 col-lg-4 mb-4 d-flex flex-column justify-content-start align-items-center mb-3 mb-lg-0">
                <div class="step-number mb-3">
                    <span class="badge rounded-pill">1</span>
                </div>
                <div class="text-center">
                    <h3>Inscription & visa</h3>
                    <p>Vous créez votre espace bailleur et le locataire fournit son visa Visale, certifié par Action Logement.</p>
                </div>
        </div>
        
        <!-- Étape 2 -->
        <div class="workflow-step col-12 col-lg-4 mb-4 d-flex flex-column justify-content-start align-items-center mb-3 mb-lg-0">
            <div class="step-number mb-3">
              <span class="badge rounded-pill">2</span>
            </div>
            <div class="text-center">
                <h3>Validation du visa</h3>
                <p>Vous saisissez le numéro de visa, vérifiez les données et remplissez les informations du logement.</p>
            </div>
        </div>
        
        <!-- Étape 3 -->
        <div class="workflow-step col-12 col-lg-4 mb-4 d-flex flex-column justify-content-start align-items-center mb-3 mb-lg-0">
            <div class="step-number mb-3">
              <span class="badge rounded-pill">3</span>
            </div>
            <div class="text-center">
                <h3>Signature du contrat</h3>
                <p>Vous acceptez le contrat de cautionnement Visale. Le contrat est immédiatement disponible.</p>
            </div>
        </div>
      </div>
      
    </div>
  </section>
</template>

<script>
export default {
  name: 'WorkFlow'
}
</script>

<style scoped>
.workflow {
  background-color: #E1E2F8;
}

.workflow h2 {
  color: #193B68;
  font-size: 40px;
  font-weight: 600;
  margin-bottom: 80px;
}

.workflow-step:hover {
  transform: translateY(-5px);
  transition: transform 0.2s ease;
}

.step-number .badge {
  width: 80px;
  height: 80px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 40px;
  font-weight: bold;
  background-color: #009EE3;
  color: white;
}

.workflow-step h3{
    color: #E6224B;
    font-size: 18px;
    font-style: normal;
    font-weight: 600;
    line-height: 60px;
  }

  .workflow-step p{
    color: #000;
    font-size: 14px;
    font-style: normal;
    font-weight: 400;
  }
</style>
