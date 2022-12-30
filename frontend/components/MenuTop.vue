<template>
  <div class="bandeau">
    <img :src="logoSrc" alt="Accueil" class="w20p bandeau-img fleft" />
    <div class="menu-items">
      <nav class="crumbs">
        <ul>
            <li class="crumb"><a @click="selectMenu($event, 'about')">Notre société</a></li>
            <li class="crumb"><a @click="selectMenu($event, 'pandas')">Nos pandas</a></li>
            <li class="crumb"><a @click="selectMenu($event, 'join')">Nous rejoindre</a></li>
            <li class="crumb"><a @click="selectMenu($event, 'contact')">Contact</a></li>
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
      selectMenu: function (event, route) {
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