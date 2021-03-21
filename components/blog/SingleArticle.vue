<template>
  <div class="bg-gray-light">
    <img alt="img" :src="pic" :alt="pic" class="h-64 w-full object-cover">
    <div class="px-10 py-6 text-center">
      <span class="text-blue font-bold uppercase">{{ category }}</span>
      <p class="font-bold text-verylarge">
        {{ title }}
      </p>
      <p class="py-2 text-gray-dark px-2 ">
        {{ summary }}
      </p>
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
