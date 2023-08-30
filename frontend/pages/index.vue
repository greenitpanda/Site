<template>
  <div style="width: 100vw;overflow: hidden">
    <MenuTop />
    <div id="content" class="content">
      <NuxtChild />
    </div>
    <MenuBottom />
  </div>
</template>
<link rel="preload" as="font" href="./assets/fonts/Poppins-Regular.ttf" type="font/ttf" crossorigin="anonymous"></link>
<link rel="preload" as="font" href="./assets/fonts/Poppins-Bold.ttf" type="font/ttf" crossorigin="anonymous"></link>
<link rel="preload" as="font" href="./assets/fonts/Poppins-Light.ttf" type="font/ttf" crossorigin="anonymous"></link>
<script>

export default {
  name: 'IndexPage',
  mounted() {
    document.title = "Green IT Panda"
  }
}
</script>
