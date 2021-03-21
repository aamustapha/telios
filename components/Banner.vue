<template>
  <div v-bind="$attrs" style="background-image: url('https://ik.imagekit.io/hooli/telios/Group_9_gWLuwYdrMs.png')" class="bg-center relative text-white mb-24">
    <div class="absolute h-full w-full bg-black top-0 bottom-0 py-2 bg-opacity-25" />
    <div class="container container-fluid py-12">
      <Navigation />
      <slot />
    </div>
  </div>
</template>

<script>
import Navigation from "~/components/Navigation"
export default {
  name: "Banner",
  components: { Navigation }
}
</script>

<style scoped>

</style>
