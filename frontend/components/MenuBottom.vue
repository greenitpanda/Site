<template>
  <div class="w100p backgroundBottom">
    <div><img :src="logoSrcSansFond" class="logoBackgroundBottom" /></div>
    <div><img :src="empreinte" class="empreinte" /></div>
    <div id="projetQuestion" class="greyBorder w80p ml10p pt50 box">
      <div class="boxElement boxLine">
        <div>
          <div class="exert">Un projet, une question ?</div>
          <div class="exert2">N'hésitez pas à nous contacter !</div>
        </div>
      </div>
      <div class="boxElement boxLine">
        <a href="/contact" class="contactButtonBottom"><span>NOUS CONTACTER</span></a>
      </div>
    </div>
    <div id="contactBandeau" class="infoEntreprise w80p ml10p box">
      <hr class="separator w5p m20 boxElement"/>
      <div id="contactLinkedin" class="contact boxElement box">
        <a href="https://www.linkedin.com/in/florian-collonge-072196ba/">
          <div class="logoLinkedin boxElement">
            in
          </div>
        </a>
        <a href="https://www.linkedin.com/in/florian-collonge-072196ba/">
          <div class="contactText boxElementDouble">Suivez-nous sur LinkedIn</div>
        </a>
      </div>
      <hr class="separator w5p m20 boxElement"/>
      <div id="contactTel" class="contact boxElementTriple box">
        <div class="contactText boxElement">Contactez-nous par téléphone</div>
        <div class="contactTel boxElementDouble">+33 3 85 72 48 59</div>
      </div>
      <hr class="separator w5p m20 boxElementTriple"/>
    </div>
    <div id="infoEntreprise" class="infoEntreprise w80p ml10p box">
      <div id="ecoindex" class="boxElement"></div>
      <div class="boxElement">
        <nuxt-link to="/"><img :src="logoSrc" alt="Accueil" class="logoBottom" /></nuxt-link>
      </div>
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
  </div>
</template>

<script>
  import logoSrc from "@/assets/images/LOGO_NOIR&BLANC.png";
  import logoSrcSansFond from "@/assets/images/LOGO_NOIR&BLANC_SANSFOND.png";
  import empreinte from "@/assets/images/forme-contact.svg";

  export default({
    name: "MenuBottom",
    setup() {
      return {
        logoSrc,
        logoSrcSansFond,
        empreinte
      };
    },
    methods: {
      selectMenu: function (event) {
        const currentActive = document.querySelector('a[aria-current="true"]');
        if (currentActive)
          currentActive.ariaCurrent = false;
        event.currentTarget.ariaCurrent = true;
        window.scrollTo(0, 0);
      }
    }
  });
</script>

<style scoped>
@import "@/assets/css/menuBottom.css"
</style>