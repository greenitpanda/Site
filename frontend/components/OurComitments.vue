<template>
  <div class="comitmentContainer">
    <div class="boxElement containerIllustration">
      <img class="illustration" :src="background" />
      <img class="illustrationPicto" :src="pictoEngagement" />
      <div class="textIllustration"><span>Repenser votre projet pour une solution plus responsable et durable</span></div>
    </div>
    <div class="comitments boxElement">
      <div class="infoComitment">
        <span class="sectionTitle">Notre engagement</span>
        <h1>Le Green It au cœur de notre démarche</h1>
        <span class="sectionText">Green It Panda vous propose des solutions numériques moins gourmandes en énergies, plus respectueuses de l'environnement, et plus centrées sur les besoins des utilisateurs.</span>
        <div class="mt30"><nuxt-link class="button" to="/contact"><span>JE ME RENSEIGNE</span></nuxt-link></div>
      </div>
    </div>
  </div>
</template>

<script>
  import background from "@/assets/images/comitment.png";
  import pictoEngagement from "@/assets/images/picto-engagement.svg";
  export default {
    name: 'OurComitments',
    setup() {
      return {
        background,
        pictoEngagement
      };
    }
  }
</script>

<style scoped>
  @import "@/assets/css/comitment.css"
</style>