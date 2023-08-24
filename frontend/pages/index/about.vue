<template>
  <div>
    <HookEntry/>
    <OurServices />
    <OurComitments />
    <OurHistory />
    <UsefulDatas />
  </div>
</template>

<script>

  import logoSrcSansFond from "@/assets/images/LOGO_NOIR_BLANC_SANSFOND.svg";
  export default {
    name: 'Accueil',
    setup() {
      return {
        logoSrcSansFond
      };
    }
  }
</script>

<style scoped>
  @import "@/assets/css/index.css"
</style>