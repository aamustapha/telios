<template>
  <div v-bind="$attrs" style="background-image: url('images/Group 9.png')" class="bg-cover text-white mb-24">
    <div class="container mx-auto py-5">
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
