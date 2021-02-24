<template>
  <div class="bg-gray-light">
    <img :src="pic" class="h-64 w-full object-cover">
    <div class="px-12 py-6 text-center">
      <span class="text-blue font-bold text-sm uppercase">{{ category }}</span>
      <p class="font-bold">
        {{ title }}
      </p>
      <small class="py-2 text-gray-dark "> {{ summary }}</small>
    </div>
  </div>
</template>

<script>
export default {
  name: "SingleArticle",
  props: {
    pic: { type: String, required: true },
    category: { type: String, required: true },
    title: { type: String, required: true },
    summary: { type: String, required: true }
  }
}
</script>

<style scoped>

</style>
