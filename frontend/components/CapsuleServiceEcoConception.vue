<template>
  <div class="capsule">
    <div>
      <div class="icon">
        <img :src="logoIcon" />
      </div>
    </div>
    <div class="sectionText w70p">Ecoconception numérique</div>
    <div>
      <nuxt-link class="capsuleButton" to="/ecoconception"><span>Découvrir</span></nuxt-link>
    </div>
  </div>
</template>

<script>
  import logoIcon from "@/assets/images/icon_ecoconception.png";
  export default {
    name: 'CapsuleServiceEcoconception',
    setup() {
      return {
        logoIcon
      };
    }
  }
</script>

<style scoped>
  @import "@/assets/css/capsuleService.css";
</style>