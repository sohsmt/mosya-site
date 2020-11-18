<template>
  <div>
    <div class="container">
      <Header />
      <Nuxt />
      <Footer />
    </div>
  </div>
</template>

<script>
export default {
  head() {
    return {
      htmlAttrs: {
        lang: 'ja',
      },
    }
  },
}
</script>

<style></style>
