<template>
  <div class="capsule">
    <div>
      <div class="icon">
        <img :src="logoIconDev" />
      </div>
    </div>
    <div class="sectionText w70p">Ecoconception numérique</div>
    <div>
      <a href="#" class="capsuleButton"><span>Découvrir</span></a>
    </div>
  </div>
</template>

<script>
  import logoIconDev from "@/assets/images/icon_dev.png";
  export default {
    name: 'CapsuleServiceEcoconception',
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