<template>
  <div style="background-image: url('images/chris-lee-70l1tDAI6rM-unsplash.png')" class="bg-cover py-24 relative">
    <div class="absolute w-full h-full bg-black bg-opacity-50 z-0" style="top: 0;"><!-- overlay --></div>
    <div class="relative container mx-auto z-10 ">
      <h5 class="text-blue-400">About us</h5>
      <h2 class="font-black text-5xl mt-2 mb-4 max-w-lg text-white">We bring you the finest details</h2>
      <div class="grid grid-cols-4 gap-4">
        <template v-for="(service, index) in services">
          <Service v-bind="service" :key="index"></Service>
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
          title: "Free Wifi to stay connected",
          description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat."
        },
        {
          title: "4K Television and Netflix included",
          description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat."
        },
        {
          title: "Span zone where you can chill",
          description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat."
        },
        {
          title: "Spacious rooms for awesome parties",
          description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat."
        }
      ]
    }
  }
}
</script>

<style scoped>

</style>
