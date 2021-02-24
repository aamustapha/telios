<template>
  <div class="flex bg-gray-200">
    <img :src="pic" class="h-full w-1/4 object-cover flex-shrink-0"/>
    <div class="py-10 pl-4 pr-16">
      <span class="text-blue-600 uppercase font-semibold">{{ category }}</span>
      <p class="font-bold">{{ name }}</p>
      <small class="py-2 text-gray-700 "> {{ description }}</small>
    </div>
    <a href="#" class="w-12 h-full bg-blue-800 flex  flex-shrink-0 content-center ">
      <img src="images/arrow-right (1)-10.svg" class=" mx-auto "/>
    </a>
  </div>
</template>

<script>
export default {
  name: "SingleRoom",
  props: {
    pic: String,
    category: String,
    name: String,
    description: String
  }
}
</script>

<style scoped>

</style>
