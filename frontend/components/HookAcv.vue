<template>
  <div class="entryEntreprise">
    <div class="hook">
      <img :src="empreinte" class="empreinteHeader" />
      <div class="contentHook">
        <h1 class="textHook">
          Analyse du cycle de vie de vos systèmes d'information
        </h1>
      </div>
    </div>
  </div>
</template>

<script>

import empreinte from "@/assets/images/forme-header.svg";
  export default {
    name: 'HookCompany',
    setup() {
      return {
        empreinte
      };
    }
  }
</script>
