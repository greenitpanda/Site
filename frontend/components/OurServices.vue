<template>
  <div class="servicesContainer">
    <div class="background"><img :src="backgroundQuadrille" /></div>
    <span class="sectionTitle">Nos prestations</span>
    <div class="w50p topDisplay">
      <h1>Services numériques responsable</h1>
      <span class="sectionText">En accompagnant les entreprises dans le développement de leurs services numériques, nous leur offrons une opportunité de concilier innovation et responsabilité environnementale.</span>
    </div>
    <div class="capsules topDisplay">
      <div class="capsule">
        <CapsuleServiceDev />
      </div>
      <div class="capsule">
        <CapsuleServiceEcoConception class="capsuleEcoconception" />
      </div>
      <div class="capsule">
        <CapsuleServiceACV class="capsuleAcv" />
      </div>
    </div>
  </div>
</template>

<script>
  import backgroundQuadrille from "@/assets/images/fond_quadrillé.png";
  export default {
    name: 'OurServices',
    setup() {
      return {
        backgroundQuadrille
      };
    }
  }
</script>

<style scoped>
  @import "@/assets/css/index.css";
  @import "@/assets/css/services.css";
</style>