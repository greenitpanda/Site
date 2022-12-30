<template>
  <div class="bandeau">
    <img :src="logoSrc" alt="Accueil" class="w20p bandeau-img fleft" />
    <div class="menu-items">
      <nav class="crumbs">
        <ul>
            <li class="crumb"><nuxt-link to="/about" @click="selectMenu($event)">Notre société</nuxt-link></li>
            <li class="crumb"><nuxt-link to="/pandas" @click="selectMenu($event)">Nos pandas</nuxt-link></li>
            <li class="crumb"><nuxt-link to="/join" @click="selectMenu($event)">Nous rejoindre</nuxt-link></li>
            <li class="crumb"><nuxt-link to="/contact" @click="selectMenu($event)">Contact</nuxt-link></li>
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