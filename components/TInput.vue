<template>
  <div :class="`my-3 flex-grow`">
    <label :for="inputId" class="text-blue font-medium text-sm">{{ label }}</label>
    <input
      :id="inputId"
      v-model="val"
      v-bind="{...$attrs, class: inputClass}"
      class=" block py-3 px-5 block w-full focus:rounded-none border-2 focus:border-gray"
    >
  </div>
</template>

<script>
export default {
  name: "TInput",
  props: {
    value: { type: [String, Number], required: false, default: undefined },
    id: { type: String, required: false, default: undefined },
    label: { type: String, required: true },
    inputClass: { type: String, required: true },
    class: { type: String, required: false }
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
    },
    classes () {
      return this.class
    }
  }
}
</script>

<style scoped>

</style>
