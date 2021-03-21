<template>
  <div>
    <div class="flex mb-1 items-center">
      <div>
        <img alt="img" :src="pic" class="rounded-full" style="width: 54px; height: 54px;">
      </div>
      <div class="pl-5">
        <h4 class="font-semibold text-verylarge">
          {{ name }}
        </h4>
        <small class="font-semibold test-small opacity-50">{{ role }}</small>
      </div>
    </div>
    <div class="mt-4 max-w-sm">
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
