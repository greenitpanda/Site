<template>
  <div class="entryEntreprise">
    <div class="hook">
      <img :src="empreinte" class="empreinteHeader" />
      <div class="contentHook">
        <h1 class="textHook">
          Vous accompagner vers des services numériques plus responsables
        </h1>
      </div>
    </div>
  </div>
</template>

<script>

import empreinte from "@/assets/images/forme-header.svg";
  export default {
    name: 'HookEngagement',
    setup() {
      return {
        empreinte
      };
    }
  }
</script>