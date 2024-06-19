<template>
  <div v-if="!isMobile()" style="width: 100vw;overflow: hidden">
    <MenuTop />
    <div id="content" class="content">
      <NuxtChild />
    </div>
    <MenuBottom />
  </div>
  <div v-else style="width: 100vw;overflow: hidden;height:100vh">
    <img :src="constructing" />
  </div>
</template>
<link rel="preload" as="font" href="./assets/fonts/Poppins-Regular.ttf" type="font/ttf" crossorigin="anonymous"></link>
<link rel="preload" as="font" href="./assets/fonts/Poppins-Bold.ttf" type="font/ttf" crossorigin="anonymous"></link>
<link rel="preload" as="font" href="./assets/fonts/Poppins-Light.ttf" type="font/ttf" crossorigin="anonymous"></link>
<script>
import { isMobile } from "../assets/js/mobile"
import constructing from "@/assets/images/under_construction.jpg";
export default {
  name: 'IndexPage',
  setup() {
    return {
      constructing
    };
  },
  watch:{
    $route (to, from){
        window.scrollTo(0, 0);
    }
  },
  mounted() {
    document.title = "Green IT Panda";
  },
  methods: {
    isMobile() {
      return isMobile();
    }
  }
}
</script>
