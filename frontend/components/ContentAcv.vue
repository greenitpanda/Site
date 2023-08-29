<template>
  <div class="contentInfo">
    <div class="descriptionInfo">
      <div>
        <div class="fright">
          <img :src="backgroundSrc" alt="Think green !" />
        </div>
        <h2>
          Réduire l'empreinte environnementale de vos SI
        </h2>
        <p class="description">
          <nuxt-link to="/about">Green IT Panda</nuxt-link>, est une entreprise spécialisée dans le <b>développement de logiciels</b> et <b>l'écoconception de services numériques</b>. Notre objectif est d'accompagner les <b>entreprises</b> dans le <b>développement</b> de leurs <b>services numériques</b> en intégrant une <b>démarche</b> de <b>numérique responsable</b>.
          <br/><br/>
          Nous réalisons une <b>analyse du cycle de vie</b> sur les <b>systèmes d'informations</b> pour garantir leur <b>durabilité</b>. Cette analyse peut être réalisée en amont de <b>l'écoconception</b> et consiste en un <b>audit</b> très <b>complet</b> qui permet d'obtenir une <b>image précise</b> de <b>l'empreinte environnementale</b> de vos <b>systèmes d'information</b>.
          <br/><br/>
          <b>L'analyse du cycle de vie</b> offre une vision globale de <b>l'impact environnemental</b> de vos <b>systèmes d'information</b>, en prenant en compte toutes les ressources nécessaires à sa <b>conception</b>, sa <b>production</b>, son <b>utilisation</b> et sa <b>fin de vie</b>.
          <br/><br/>
          Pour cela, nous vous proposons des solutions pour réduire <b>l'impact environnemental</b> de vos <b>systèmes d'information</b>. En intégrant une démarche de <b>numérique responsable</b> dès la <nuxt-link to="/ecoconception">conception</nuxt-link> de vos <b>services numériques</b>, vous pouvez réduire votre <b>empreinte environnementale</b> tout en répondant aux besoins de vos utilisateurs. <b>Green IT Panda</b> vous accompagne dans cette démarche. Nos compétences en <nuxt-link to="/developpement">développement</nuxt-link>, et notre démarche <b>écoresponsable</b>, nous permettent de <b>créer</b> ou de <b>repenser</b> vos <b>services numériques</b> grâce à <b>l'écoconception</b>. Pour en savoir plus, ou pour une première approche de votre projet, <nuxt-link to="/contact">contactez-nous</nuxt-link>.
        </p>
      </div>
    </div>
  </div>
</template>

<script>

  import backgroundSrc from "@/assets/images/acv.jpg";
  export default {
    name: 'ContentCompany',
    setup() {
      return {
        backgroundSrc
      };
    }
  }
</script>
