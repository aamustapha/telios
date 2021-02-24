<template>
  <div>
    <div class="flex mb-1">
      <div>
        <img :src="pic" class="w-12 h-12 rounded-full">
      </div>
      <div class="pl-5">
        <h4 class="font-bold text-md">
          {{ name }}
        </h4>
        <small class="text-gray-dark">{{ role }}</small>
      </div>
    </div>
    <div class="mt-4">
      <p>{{ testimony }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Testimony",
  props: {
    pic: { type: String, required: true },
    name: { type: String, required: true },
    role: { type: String, required: true },
    testimony: { type: String, required: true }
  }
}
</script>

<style scoped>

</style>
