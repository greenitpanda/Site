<template>
  <div class="entryEntreprise">
    <div class="hook">
      <img :src="empreinte" class="empreinteHeader" />
      <div class="contentHook">
        <h1 class="textHook">
          Green IT Panda pour le développement de vos logiciels
        </h1>
      </div>
    </div>
  </div>
</template>

<script>

import empreinte from "@/assets/images/forme-header.svg";
  export default {
    name: 'HookDeveloppement',
    setup() {
      return {
        empreinte
      };
    }
  }
</script>