<template>
  <div>
    <Nuxt />
    <Photos />
    <Footer />
  </div>
</template>

<script>
import Footer from "~/components/Footer"
import Photos from "~/components/Photos"

export default {
  components: { Photos, Footer }
}
</script>

<style>
* {
  font-family: 'Poppins', sans-serif;
}

.container-fluid {
  @apply px-8
}
</style>
