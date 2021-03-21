<template>
  <div style="background-image: url('https://ik.imagekit.io/hooli/telios/chris-lee-70l1tDAI6rM-unsplash_hBKVMwBJOfR0.png')" class="bg-cover py-24 relative">
    <div class="absolute h-full w-full bg-black top-0 bottom-0 py-2 bg-opacity-25"></div>
    <div class="relative container container-fluid mx-auto z-10 ">
      <h5 class="text-blue uppercase font-bold">
        About us
      </h5>
      <h2 class="font-extrabold text-big mb-6 leading-tight max-w-lg text-white">
        We bring you the finest details
      </h2>
      <div class="flex gap-4">
        <template v-for="(service, index) in services">
          <Service v-bind="service" :key="index" />
        </template>
      </div>
    </div>
  </div>
</template>

<script>
import Service from "~/components/services/Service"
export default {
  name: "Services",
  components: { Service },
  data () {
    return {
      services: [
        {
          title: "Free Wifi\nto stay connected",
          description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt"
        },
        {
          title: "4K Television and\n Netflix included",
          description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt"
        },
        {
          title: "Span zone where\nyou can chill",
          description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt"
        },
        {
          title: "Spacious rooms\nfor awesome parties",
          description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt"
        }
      ]
    }
  }
}
</script>

<style scoped>

</style>
