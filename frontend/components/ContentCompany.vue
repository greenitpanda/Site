<template>
  <div class="contentInfo">
    <div class="descriptionInfo">
      <div>
        <div class="fright">
          <img :src="backgroundSrc" alt="Think green !" />
        </div>
        <h2>
          Des services moins gourmands, recentré sur vos cœurs de cible
        </h2>
        <p class="description">
          Après avoir travaillé pendant des années dans le monde du <b>logiciel</b> et avoir gravi les échelons jusqu'à devenir <b>directeur technique</b>, j'ai réalisé que le secteur était souvent déconnecté des <b>enjeux humains et environnementaux</b>. Désireux de faire bouger les choses, j'ai décidé de créer <b>Green IT Panda</b>, afin d'accompagner mes clients dans le développement de services plus responsables et durables. Mon objectif est de proposer <b>des solutions numériques moins gourmands en ressources, recentrées sur leur cœur de cible et plus accessibles pour les utilisateurs</b>.
          <br/><br/>
          <b>Green IT Panda</b> a une approche holistique qui prend en compte les aspects <b>environnementaux, humains et économiques</b>. Je suis convaincu que ces trois perspectives sont intimement liés, et que l'on peut créer des <b>services numériques</b> qui soient à la fois <b>respectueux de l'environnement</b>, accessibles et <b>rentables</b>.
          <br/><br/>
          Ainsi, <b>Green IT Panda</b> travaille à la création de <b>services numériques</b> qui consomment moins de ressources et qui sont plus efficaces pour leurs utilisateurs. <b>Green IT Panda</b> se concentre également sur <b>l'amélioration de l'accessibilité des services numériques</b>, en veillant à ce que tous les utilisateurs, y compris ceux ayant des handicaps, puissent facilement naviguer sur les sites. Enfin, je cherche à <b>diminuer</b> la <b>charge financière</b> et le <b>besoin en maintenance des services numériques</b> en proposant des <b>solutions simples</b> et <b>durables</b>. Pour cela, je suis à votre écoute pour le <nuxt-link to="/developpement">développement de logiciels</nuxt-link>, <nuxt-link to="/ecoconception">l'écoconception numérique</nuxt-link>, ainsi que pour l'<nuxt-link to="/acv">analyse du cycle de vie des systèmes d'information</nuxt-link>. <nuxt-link to="/contact">Contactez-moi</nuxt-link> pour plus d'informations.
        </p>
      </div>
    </div>
  </div>
</template>

<script>

  import backgroundSrc from "@/assets/images/interieure.jpg";
  export default {
    name: 'ContentCompany',
    setup() {
      return {
        backgroundSrc
      };
    }
  }
</script>
