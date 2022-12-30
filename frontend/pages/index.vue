<template>
  <div>
    <MenuTop />
    <div id="content" class="content">
      <NuxtChild />
    </div>
  </div>
</template>

<script>

export default {
  name: 'IndexPage',
  mounted() {
    document.title = "Green IT Panda"
  }
}
</script>
