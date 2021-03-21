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
  font-size: 14px;
}

.container-fluid {
  @apply px-2 mx-auto;
  max-width: 1140px;
}

@screen lg {
  .container-fluid {
    @apply px-8
  }
}
</style>
