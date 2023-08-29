<template>
  <div class="contentInfo">
    <div class="descriptionInfo">
      <div>
        <div class="fright">
          <img :src="backgroundSrc" alt="Think green !" />
        </div>
        <h2>
          Des technologies plus respectueuses de l'environnement
        </h2>
        <p class="description">
          Au travers de <nuxt-link to="/about">Green IT Panda</nuxt-link>, notre objectif est de proposer <b>des solutions numériques moins gourmandes en ressources, plus respectueuses de l'environnement</b>, et plus <b>centrées</b> sur les <b>besoins</b> des <b>utilisateurs</b>.
        </p>
        <h3>Notre approche repose sur trois piliers : l'environnement, l'humain, et l'économie.</h3>
        <p class="description">
          Sur le plan <b>environnemental</b>, nous mettons en place des stratégies pour limiter la <b>consommation de ressources</b> et votre <b>empreinte environnementale</b>. Nous utilisons des technologies plus <b>respectueuses de l'environnement</b> et nous encourageons les <b>pratiques écoresponsables</b> chez nos clients.
          <br/><br/>
          Sur le plan <b>humain</b>, nous nous attachons à <b>améliorer l'accessibilité</b> des <b>services numériques</b> pour tous les utilisateurs, notamment les personnes en situation de handicap. Nous travaillons également à rendre les <b>interfaces plus conviviales</b> et <b>plus adaptées</b> aux <b>besoins des utilisateurs</b>.
          <br/><br/>
          Enfin, sur le plan <b>économique</b>, nous visons à réduire la <b>charge financière</b> des <b>services numériques</b> pour nos clients en diminuant les <b>coûts de maintenance</b>. Cette approche permet également de réduire <b>l'empreinte environnementale</b> des <b>services numériques</b> en limitant les <b>besoins</b> en <b>énergie</b> et en <b>ressources</b>.
          <br/><br/>
          En accompagnant les entreprises dans le <b>développement</b> de leurs <b>services numériques</b>, nous leur offrons une opportunité de concilier <b>innovation</b> et <b>responsabilité environnementale</b>.
          <br/>
          Grâce à cette démarche de <b>numérique responsable</b>, les entreprises peuvent contribuer à <b>réduire leur impact sur l'environnement</b> tout en offrant des <b>services numériques de qualité</b> à leurs clients. Pour cela, nous les accompagnons dans le <nuxt-link to="/developpement">développement de logiciels</nuxt-link>, pour de <nuxt-link to="/ecoconception">l'écoconception numérique</nuxt-link>, ainsi que pour <nuxt-link to="/acv">l'analyse du cycle de vie des systèmes d'information</nuxt-link>. <nuxt-link to="/contact">Contactez</nuxt-link> dès maintenant Green IT Panda pour une première approche de votre projet.
        </p>
      </div>
    </div>
  </div>
</template>

<script>

  import backgroundSrc from "@/assets/images/engagement.jpg";
  export default {
    name: 'ContentEngagement',
    setup() {
      return {
        backgroundSrc
      };
    }
  }
</script>