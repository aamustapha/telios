<template>
  <div class="mb-24 flex justify-between">
    <h4 class="font-extrabold">
      Zetta Hotels
    </h4>
    <nav class="font-sm">
      <template v-for="(nav, index) in navs">
        <router-link
          :key="index"
          :to="nav.link"
          class="mx-3 uppercase font-semibold "
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
