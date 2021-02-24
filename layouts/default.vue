<template>
  <div>
    <Nuxt/>
    <Photos />
    <Footer />
  </div>
</template>
<style>
* {
  font-family: 'Poppins', sans-serif;
}
</style>
<script>
import Footer from "~/components/Footer"
import Photos from "~/components/Photos"
export default {
  components: { Photos, Footer }
}
</script>
