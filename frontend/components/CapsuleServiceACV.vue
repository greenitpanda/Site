<template>
  <div class="capsule">
    <div>
      <div class="icon">
        <img :src="logoIcon" />
      </div>
    </div>
    <div class="sectionText w70p">Analyse du cycle de vie</div>
    <div>
      <nuxt-link class="capsuleButton" to="/acv"><span>Découvrir</span></nuxt-link>
    </div>
  </div>
</template>

<script>
  import logoIcon from "@/assets/images/picto-analyse.svg";
  export default {
    name: 'CapsuleServiceACV',
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