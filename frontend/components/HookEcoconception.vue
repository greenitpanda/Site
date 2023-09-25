<template>
  <div class="entryEntreprise">
    <div class="hook">
      <img :src="empreinte" class="empreinteHeader" />
      <div class="contentHook">
        <h1 class="textHook">
          L'écoconception au service du numérique avec Green It Panda
        </h1>
      </div>
    </div>
  </div>
</template>

<script>

import empreinte from "@/assets/images/forme-header.svg";
  export default {
    name: 'HookEcoconception',
    setup() {
      return {
        empreinte
      };
    }
  }
</script>
