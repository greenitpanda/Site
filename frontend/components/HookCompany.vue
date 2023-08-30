<template>
  <div class="entryEntreprise">
    <div class="hook">
      <img :src="empreinte" class="empreinteHeader" />
      <div class="contentHook">
        <h1 class="textHook">
          Green IT Panda, développement de logiciels écoresponsables
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
