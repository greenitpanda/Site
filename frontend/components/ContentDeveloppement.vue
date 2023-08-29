<template>
  <div class="contentInfo">
    <div class="descriptionInfo">
      <div>
        <div class="fright">
          <img :src="backgroundSrc" alt="Think green !" />
        </div>
        <h2>
          Vos logiciels écoconçus par un professionnel
        </h2>
        <p class="description">
          Notre cœur de métier a toujours été le <b>développement de logiciels</b>, et c'est un axe que nous souhaitons continuer d'aborder. Nous avons travaillé dans plusieurs secteurs d'activité.
          <br/><br/>
          Nous avons notamment conçu un <b>logiciel de gestion hospitalier</b>, pour permettre aux professionnels de santé de <b>centraliser</b> et <b>d'améliorer</b> les <b>parcours de soins</b> de leurs patients (Gestion des parcours infirmiers, gestion des prescriptions, du dossier médical patient, etc.). Outre la gestion des hôpitaux, nous avons également développé des <b>logiciels de gestion des promotions</b> dans la grande distribution ainsi que des <b>solutions de facturation</b> des patients pour les hôpitaux. Nous avons travaillé sur la <b>plateforme de paiement</b> d'un grand groupe bancaire, permettant aux clients de réaliser des transactions financières en ligne en toute sécurité.
          <br/><br/>
          Aujourd'hui <nuxt-link to="/about">Green IT Panda</nuxt-link> intervient pour <nuxt-link to="/ecoconception">l'écoconception numérique</nuxt-link>, ainsi que pour <nuxt-link to="/acv">l'analyse du cycle de vie</nuxt-link> de vos <b>systèmes d'information</b>. 
          <br/><br/>
          Avec <b>Green IT Panda</b>, nous souhaitons conserver cette ambition de porter le <b>Green IT</b> au travers des <b>logiciels</b> que nous développons. Aujourd'hui, le <b>Green IT</b> est une réponse adaptée aux <b>défis environnementaux</b> auxquels les entreprises sont confrontées. En adoptant ces <b>technologies</b>, les <b>entreprises</b> peuvent <b>améliorer</b> leur <b>image de marque</b> et leur <b>réputation</b>, en montrant leur <b>engagement</b> en faveur du <b>développement durable</b>. <nuxt-link to="/contact">Contactez Green IT Panda</nuxt-link> dès maintenant pour plus de renseignements.
        </p>
      </div>
    </div>
  </div>
</template>

<script>

  import backgroundSrc from "@/assets/images/developpement.jpg";
  export default {
    name: 'ContentDeveloppement',
    setup() {
      return {
        backgroundSrc
      };
    }
  }
</script>
