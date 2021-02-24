<template>
  <div>
    <div class="container mx-auto">
      <h5 class="text-blue uppercase font-bold">
        photos
      </h5>
      <h2 class="font-black text-4xl mt-2 mb-4 max-w-lg">
        See our latest photos from restaurant and hotel
      </h2>
    </div>
    <div class="grid grid-cols-4 h-64">
      <img v-for="(src, index) in images" :key="index" :src="src" class="object-cover w-full h-full">
    </div>
  </div>
</template>

<script>
export default {
  name: "Photos",
  data () {
    return {
      images: [
        "images/mohamed-ajufaan-GFcWwwGNu_w-unsplash.png",
        "images/manuel-moreno-DGa0LQ0yDPc-unsplash.png",
        "images/rhema-kallianpur-jbJ-_hw2yag-unsplash.png",
        "images/eddi-aguirre-ZAVHbpOn4Jk-unsplash.png"
      ]
    }
  }
}
</script>

<style scoped>

</style>
