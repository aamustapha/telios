<template>
  <div class="bg-gray-200">
    <img :src="pic" class="h-64 w-full object-cover"/>
    <div class="px-12 py-6 text-center">
      <span class="text-blue-600 font-bold text-sm uppercase">{{ category }}</span>
      <p class="font-bold">{{ title }}</p>
      <small class="py-2 text-gray-700 "> {{ summary }}</small>
    </div>
  </div>
</template>

<script>
export default {
  name: "SingleArticle",
  props: {
    pic: String,
    category: String,
    title: String,
    summary: String
  }
}
</script>

<style scoped>

</style>
