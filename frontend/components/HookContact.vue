<template>
  <div class="entryContact">
    <div class="hook">
      <img :src="empreinte" class="empreinteHeader" />
      <div class="contentHook">
        <h1 class="textHook">
          Contactez-nous dès maintenant : nous sommes à l'écoute de vos besoins pour le développement de logiciels écoconçus respectueux de l'environnement.
        </h1>
      </div>
    </div>
  </div>
</template>

<script>

import empreinte from "@/assets/images/forme-header.svg";
  export default {
    name: 'HookContact',
    setup() {
      return {
        empreinte
      };
    }
  }
</script>