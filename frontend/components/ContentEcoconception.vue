<template>
  <div class="contentInfo">
    <div class="descriptionInfo">
      <div>
        <div class="fright">
          <img :src="backgroundSrc" alt="Think green !" />
        </div>
        <h2>
          Audit, refonte et création de vos services numériques
        </h2>
        <p class="description">
          <b>L'écoconception numérique</b>, est une approche qui vise à <b>réduire l'impact environnemental</b> des <b>technologies de l'information</b> et de la <b>communication.</b> 
          <br/><br/>
          Cette méthode consiste à <b>concevoir</b>, avec <nuxt-link to="/about">Green IT Panda</nuxt-link>, des <b>services</b> ou des <b>applications numériques</b> de manière à <b>minimiser leur consommation de ressources</b> et à <b>réduire leur empreinte environnementale</b>, tout au long de leur <b>cycle de vie</b>.
          <br/><br/>
          Grâce à nos <b>compétences techniques</b>, et à notre <b>engagement environnemental</b>, nous pouvons réaliser une <b>création</b>, un <b>audit</b>, ou une <b>refonte</b> de vos <b>projets numériques</b>. Ainsi, nous pouvons vous accompagner dans toutes les étapes de votre <b>projet numérique</b>. Grâce à notre <b>expertise</b> en <b>écoconception</b>, nous pouvons vous aider à concevoir des <b>projets numériques écoresponsables</b>, en prenant en compte les <b>enjeux environnementaux</b> dès la phase de <b>conception</b>.
          <br/><br/>
          Si vous avez déjà un <b>projet numérique</b> en place, nous pouvons également réaliser un <b>audit</b> pour évaluer son <b>impact environnemental</b> et vous <b>proposer des solutions</b> pour le rendre plus <b>écoresponsable</b>. Enfin, si votre <b>projet numérique</b> nécessite une <b>refonte</b>, nous pouvons vous accompagner dans cette démarche en proposant des <b>solutions innovantes</b> et <b>respectueuses de l'environnement</b>.
          <br/><br/>
          En adoptant une approche <b>d'écoconception numérique</b>, les entreprises peuvent réduire leur <b>empreinte environnementale</b>. En outre, une <b>conception numérique</b> plus durable peut également offrir des <b>avantages financiers</b> tels que des <b>économies d'énergie</b>, des <b>coûts de maintenance réduits</b> et une <b>amélioration</b> de la <b>réputation</b> de l'entreprise. 
          <br/><br/>
          Pour en savoir plus, <nuxt-link to="/contact">contactez-nous</nuxt-link> dès maintenant.
        </p>
      </div>
    </div>
  </div>
</template>

<script>

  import backgroundSrc from "@/assets/images/ecoconception.jpg";
  export default {
    name: 'ContentEcoconception',
    setup() {
      return {
        backgroundSrc
      };
    }
  }
</script>
