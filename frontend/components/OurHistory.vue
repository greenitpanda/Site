<template>
  <div class="historyContainer">
    <img :src="tetePanda" class="panda" />
    <img :src="empreinte" class="whitePrint" />
    <img :src="arrow" class="arrowBottom" />
    <div class="pandaEar" />
    <div class="infoHistory">
      <h1>Green IT Panda vous accompagne dans vos projets de développement logiciel, et d'accompagnement au numérique responsable </h1>
      <span>
        <nuxt-link to="/">Green IT Panda</nuxt-link> a été créée en <b>2021</b> par <b>Florian Collonge</b>. Développeur dans l'âme, il a choisi d'ancrer sa société dans un esprit de responsabilité, pour aider les entreprises à mettre en place un ensemble de techniques visant à réduire <b>l'empreinte sociale, économique</b> et <b>environnementale du numérique</b>. 
      </span>
      <br />
      <br />
      <span>
        Pour aider nos clients à atteindre cet objectif, nous réalisons <b>l'analyse du cycle de vie</b> de leurs <nuxt-link to="/acv">Systèmes d'information</nuxt-link>, ainsi que de <nuxt-link to="/ecoconception">l'écoconception numérique</nuxt-link> de manière à minimiser leur impact environnemental. N'hésitez pas à <nuxt-link to="/contact">nous contacter</nuxt-link> pour obtenir plus de renseignements.
      </span>
    </div>
  </div>
</template>

<script>
  import tetePanda from "@/assets/images/tete_panda.png";
  import empreinte from "@/assets/images/white-print.png";
  import arrow from "@/assets/images/arrow_to_left.png";
  export default {
    name: 'OurHistory',
    setup() {
      return {
        tetePanda,
        empreinte,
        arrow
      };
    }
  }
</script>

<style scoped>
  @import "@/assets/css/history.css"
</style>