<template>
  <div class="flex bg-gray-light h-48">
    <img alt="img" :src="pic" class="h-full w-1/3 object-cover flex-shrink-0 self-stretch">
    <div class="py-8 pl-8 pr-16 mr-5">
      <span class="text-blue uppercase font-semibold">{{ category }}</span>
      <p class="font-semibold text-verylarge">
        {{ name }}
      </p>
      <small class="py-2 text-gray-dark "> {{ description }}</small>
    </div>
    <a href="#" class="w-16 h-full bg-blue flex  flex-shrink-0 content-center ">
      <img alt="img" src="https://ik.imagekit.io/hooli/telios/arrow-right_-QqySiOJBG.svg" class=" mx-auto px-6 ">
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
