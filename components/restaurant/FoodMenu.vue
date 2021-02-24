<template>
  <div class="flex bg-gray-200 relative">
    <img :src="pic" class="h-full w-1/4 object-cover"/>
    <div class="py-10 pl-4 pr-16">
      <span class="text-blue-600 uppercase font-semibold">{{ category }}</span>
      <p class="font-bold">{{ name }}</p>
      <small class="py-2 text-gray-700 "> {{ description }}</small>
      <a href="#" class="absolute bottom-0 right-0">
        <img src="images/arrow-right (1)-10.svg" class="px-5 py-4 bg-blue-800"/>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "FoodMenu",
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
