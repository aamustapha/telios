<template>
  <div class="mb-24 flex justify-between relative">
    <h4 class="font-semibold text-base">
      Zetta Hotels
    </h4>
    <nav class="text-small flex gap-12">
      <template v-for="(nav, index) in navs">
        <router-link
          :key="index"
          :to="nav.link"
          class="uppercase"
          exact-active-class="text-blue"
        >
          {{ nav.text }}
          <img v-if="nav.children" src="images/chevron-down.svg" class="flex w-3 ml-1 h-2 align-middle inline-flex">
        </router-link>
      </template>
    </nav>
  </div>
</template>

<script>
import navs from "./_nav"

export default {
  name: "Navigation",
  data () {
    return {
      navs
    }
  }
}
</script>

<style scoped>

</style>
