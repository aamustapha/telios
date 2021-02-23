<template>
  <div class="bg-white py-6 px-6 text-center ">
    <span class="w-16 h-16 p-3 rounded-full bg-blue-800 mx-auto mb-3 block">
      <img src="images/001-hotel-1.svg" class="d-block mx-auto">
    </span>
    <h5 class="font-bold mb-2 text-xl">{{ title }}</h5>
    <small>{{ description }}</small>
  </div>
</template>

<script>
export default {
  name: "Service",
  props: {
    description: String,
    title: String
  }
}
</script>

<style scoped>

</style>
