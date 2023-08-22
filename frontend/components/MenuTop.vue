<template>
  <div class="bandeau">
    <img :src="logoSrc" alt="Accueil" class="w20p bandeau-img fleft" />
    <div class="menu-items">
      <nav class="crumbs">
        <ul>
            <li class="crumb"><nuxt-link to="/about" @click="selectMenu($event)">L'entreprise</nuxt-link></li>
            <li class="crumb"><nuxt-link to="/engagement" @click="selectMenu($event)">Engagement</nuxt-link></li>
            <li class="crumb"><nuxt-link to="/developpement" @click="selectMenu($event)">Développement logiciel</nuxt-link></li>
            <li class="crumb"><nuxt-link to="/ecoconception" @click="selectMenu($event)">Ecoconception numérique</nuxt-link></li>
            <li class="crumb"><nuxt-link to="/acv" @click="selectMenu($event)">Analyse du cycle de vie</nuxt-link></li>
            <li class="crumbButton"><nuxt-link to="/contact" @click="selectMenu($event)"><span class="contact">Contact</span></nuxt-link></li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<script>
  // Please just use `@` to refer to the root "src" directory of the project
  import logoSrc from "@/assets/images/LOGO_NOIR&BLANC.svg";

  export default({
    name: "MenuTop",
    setup() {
      return {
        logoSrc
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
@import "@/assets/css/menuTop.css"
</style>