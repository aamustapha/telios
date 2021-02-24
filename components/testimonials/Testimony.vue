<template>
  <div>
    <div class="flex mb-1">
      <div>
        <img :src="pic" class="w-12 h-12 rounded-full" />
      </div>
      <div class="pl-5">
        <h4 class="font-bold text-md">{{ name }}</h4>
        <small class="text-gray-800">{{ role }}</small>
      </div>
    </div>
    <div>
      <p>{{ testimony }}</p>
    </div>
  </div>

</template>

<script>
export default {
  name: "Testimony",
  props: {
    pic: String,
    name: String,
    role: String,
    testimony: String
  }
}
</script>

<style scoped>

</style>
