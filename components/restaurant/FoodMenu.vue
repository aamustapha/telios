<template>
  <div class="flex bg-gray-light relative">
    <img :src="pic" class="h-full object-cover" style="width: 168px" :alt="name">
    <div class="py-8 pl-4 pr-32">
      <span class="text-blue uppercase font-semibold">{{ category }}</span>
      <p class="font-bold text-large">
        {{ name }}
      </p>
      <p class="py-2 text-base text-gray-dark">
        {{ description }}
      </p>
      <a href="#" class="absolute bottom-0 right-0">
        <img
          src="https://ik.imagekit.io/hooli/telios/arrow-right-white_20BPr8tUO2.svg"
          alt="learn more"
          class="p-6 bg-blue"
        >
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "FoodMenu",
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
