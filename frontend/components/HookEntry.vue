<template>
  <div class="entryAbout">
    <div><img :src="arrow" class="arrow" /></div>
    <img :src="empreinte" class="empreinteHeader" />
    <div class="hook">
      <div class="contentHook">
        <h1 class="textHook">
          Un accompagnement dans vos services numériques en intégrant une démarche de <b>numérique responsable</b>
        </h1>
        <div>
          <nuxt-link to="/contact" class="contactButton" @click="selectMenu($event)"><span class="contact">NOUS CONTACTER</span></nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

  import logoSrcSansFond from "@/assets/images/LOGO_NOIR_BLANC_SANSFOND.svg";
  import arrow from "@/assets/images/arrow_to_bottom.png";
  import empreinte from "@/assets/images/forme-header.svg";
  export default {
    name: 'HookEntry',
    setup() {
      return {
        logoSrcSansFond,
        arrow,
        empreinte
      };
    }
  }
</script>

<style scoped>
  @import "@/assets/css/index.css"
</style>