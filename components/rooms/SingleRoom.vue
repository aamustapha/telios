<template>
  <div class="flex bg-gray-light">
    <img alt="img" :src="pic" class="h-full w-1/4 object-cover flex-shrink-0">
    <div class="py-10 pl-4 pr-16">
      <span class="text-blue uppercase font-semibold">{{ category }}</span>
      <p class="font-bold">
        {{ name }}
      </p>
      <small class="py-2 text-gray-dark "> {{ description }}</small>
    </div>
    <a href="#" class="w-12 h-full bg-blue flex  flex-shrink-0 content-center ">
      <img alt="img" src="images/arrow-right (1)-10.svg" class=" mx-auto ">
    </a>
  </div>
</template>

<script>
export default {
  name: "SingleRoom",
  props: {
    pic: { type: String, required: true },
    category: { type: String, required: true },
    name: { type: String, required: true },
    description: { type: String, required: true }
  }
}
</script>

<style scoped>

</style>
