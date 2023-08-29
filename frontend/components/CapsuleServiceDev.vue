<template>
  <div class="capsule">
    <div>
      <div class="icon">
        <img :src="logoIconDev" />
      </div>
    </div>
    <div class="sectionText w70p">Développement logiciel</div>
    <div>
      <nuxt-link class="capsuleButton" to="/developpement"><span>Découvrir</span></nuxt-link>
    </div>
  </div>
</template>

<script>
  import logoIconDev from "@/assets/images/picto-dev.svg";
  export default {
    name: 'CapsuleServiceDev',
    setup() {
      return {
        logoIconDev
      };
    }
  }
</script>

<style scoped>
  @import "@/assets/css/capsuleService.css";
</style>