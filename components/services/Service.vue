<template>
  <div class="bg-white py-8 px-4 text-center ">
    <div class="w-16 h-16 p-3 rounded-full bg-blue mx-auto mb-3 block">
      <img src="https://ik.imagekit.io/hooli/telios/hotel_srtzCUnOr6.svg" class="d-block mx-auto">
    </div>
    <p class="font-bold mb-4 text-verylarge whitespace-pre-line">{{ title }}</p>
    <small class="text-gray-dark text-base px-2 max-3-lines" >{{ description }}</small>
  </div>
</template>

<script>
export default {
  name: "Service",
  props: {
    description: { type: String, required: true },
    title: { type: String, required: true }
  }
}
</script>

<style scoped>
.max-3-lines{
  display: -webkit-box;
  -webkit-line-clamp: 3;
  -webkit-box-orient: vertical;
  overflow: hidden;
}
</style>
