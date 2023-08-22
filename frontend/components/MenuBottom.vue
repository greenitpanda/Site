<template>
  <div class="w100p backgroundBottom">
    <div><img :src="logoSrcSansFond" class="logoBackgroundBottom" /></div>
    <div id="projetQuestion" class="greyBorder w80p ml10p pt50 box">
      <div class="boxElement boxLine">
        <div>
          <div class="exert">Un projet, une question ?</div>
          <div class="exert2">N'hésitez pas à nous contacter !</div>
        </div>
      </div>
      <div class="boxElement boxLine">
        <a href="#" class="contactButton"><span>NOUS CONTACTER</span></a>
      </div>
    </div>
    <div id="contactBandeau" class="infoEntreprise w80p ml10p box">
      <hr class="separator w5p m20 boxElement"/>
      <div id="contactLinkedin" class="contact boxElement box">
        <div class="logoLinkedin boxElement">
          in
        </div>
        <div class="contactText boxElementDouble">Suivez-nous sur LinkedIn</div>
      </div>
      <hr class="separator w5p m20 boxElement"/>
      <div id="contactTel" class="contact boxElementTriple box">
        <div class="contactText boxElement">Contactez-nous par téléphone</div>
        <div class="contactTel boxElementDouble">+33 6 86 01 62 59</div>
      </div>
      <hr class="separator w5p m20 boxElementTriple"/>
    </div>
    <div id="infoEntreprise" class="infoEntreprise w80p ml10p box">
      <div id="ecoindex" class="boxElement">EcoIndex X</div>
      <div class="boxElement"><img :src="logoSrc" alt="Accueil" class="logoBottom" /></div>
      <div id="menu" class="boxElement">
        <ul>
            <li class="crumb"><nuxt-link to="/about" @click="selectMenu($event)">L'entreprise</nuxt-link></li>
            <li class="crumb"><nuxt-link to="/engagement" @click="selectMenu($event)">Engagement</nuxt-link></li>
            <li class="crumb"><nuxt-link to="/developpement" @click="selectMenu($event)">Développement logiciel</nuxt-link></li>
            <li class="crumb"><nuxt-link to="/ecoconception" @click="selectMenu($event)">Ecoconception numérique</nuxt-link></li>
            <li class="crumb"><nuxt-link to="/acv" @click="selectMenu($event)">Analyse du cycle de vie</nuxt-link></li>
            <li class="crumb"><nuxt-link to="/contact" @click="selectMenu($event)">Contact</nuxt-link></li>
        </ul>
      </div>
    </div>
    <div class="infosBottom">
      <ul class="crumbsInfo">
        <li class="crumbInfo"><nuxt-link to="/about" @click="selectMenu($event)">Données personnelles</nuxt-link></li>
        <li class="crumbInfo"><nuxt-link to="/engagement" @click="selectMenu($event)">Mentions légales</nuxt-link></li>
        <li class="crumbInfo"><nuxt-link to="/developpement" @click="selectMenu($event)">Cookies</nuxt-link></li>
        <li class="crumbInfo"><nuxt-link to="/ecoconception" @click="selectMenu($event)">Plan de site</nuxt-link></li>
        <li class="crumbInfo">Designé par Publigo</li>
        <li class="crumbInfo">Développé par Green IT Panda</li>
      </ul>
    </div>
  </div>
</template>

<script>
  // Please just use `@` to refer to the root "src" directory of the project
  import logoSrc from "@/assets/images/LOGO_NOIR&BLANC.png";
  import logoSrcSansFond from "@/assets/images/LOGO_NOIR&BLANC_SANSFOND.png";

  export default({
    name: "MenuBottom",
    setup() {
      return {
        logoSrc,
        logoSrcSansFond
      };
    },
    methods: {
      selectMenu: function (event) {
        const currentActive = document.querySelector('a[aria-current="true"]');
        if (currentActive)
          currentActive.ariaCurrent = false;
        event.currentTarget.ariaCurrent = true;
      }
    }
  });
</script>

<style scoped>
@import "@/assets/css/menuBottom.css"
</style>