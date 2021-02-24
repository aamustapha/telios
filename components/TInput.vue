<template>
  <div class="my-3">
    <label :for="inputId" class="text-blue-800">{{ label }}</label>
    <input
        :id="inputId"
        v-model="val"
        v-bind="{...$attrs, class: inputClass}"
        class=" block py-3 px-5 block w-full focus:rounded-none border-2 focus:border-gray-600"/>
  </div>
</template>

<script>
export default {
  name: "TInput",
  props: {
    value: [String, Number],
    id: String,
    label: { type: String, required: true },
    inputClass: {}
  },
  computed: {
    inputId () {
      return this.id || this.label.replace(/[\W_]+/g, "_")
    },
    val: {
      get () {
        return this.value
      },
      set (value) {
        this.$emit("input", value)
      }
    }
  }
}
</script>

<style scoped>

</style>
