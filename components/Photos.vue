<template>
  <div>
    <div class="container container-fluid mx-auto">
      <h5 class="text-blue uppercase font-bold">
        photos
      </h5>
      <h2 class="font-black text-big mt-2 mb-8">
        See our latest photos <br> from restaurant and hotel
      </h2>
    </div>
    <div class="flex items-center">
      <div class="z-10 h-16">
        <a href="#" class="absolute left-0 ml-16">
          <img src="https://ik.imagekit.io/hooli/telios/arrow-right-white_20BPr8tUO2.svg" alt="arrow" class="p-6 bg-blue transform rotate-180 opacity-25">
        </a>
        <a href="#" class="absolute right-0 mr-16">
          <img src="https://ik.imagekit.io/hooli/telios/arrow-right_-QqySiOJBG.svg" alt="arrow" class="p-6 bg-blue ">
        </a>
      </div>
      <div class="grid grid-cols-4 w-full">
        <img v-for="(src, index) in images" :key="index" :src="src" :alt="src" class="object-cover w-full h-full">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Photos",
  data () {
    return {
      images: [
        "https://ik.imagekit.io/hooli/telios/mohamed-ajufaan-GFcWwwGNu_w-unsplash-1_H9JkFGAwxQ.png",
        "https://ik.imagekit.io/hooli/telios/manuel-moreno-DGa0LQ0yDPc-unsplash_9lKrMYU9AzOso.png",
        "https://ik.imagekit.io/hooli/telios/rhema-kallianpur-jbJ-_hw2yag-unsplash-1_0-x8lDdAKAvkl.png",
        "https://ik.imagekit.io/hooli/telios/eddi-aguirre-ZAVHbpOn4Jk-unsplash_vVS3cvklPO4c.png"
      ]
    }
  }
}
</script>

<style scoped>

</style>
