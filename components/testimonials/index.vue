<template>
  <div class="bg-gray-200 relative flex">
    <div class="container mx-auto pr-24">
      <div>
        <div class="max-w-lg py-24">
          <h5 class="text-blue-400 uppercase font-bold">
            Testimonials
          </h5>
          <h2 class="font-black text-4xl mb-4">We trust our customers and they trust us too</h2>
          <Testimonies v-model="testimony"/>
        </div>
      </div>
    </div>

    <div
        class="w-1/3 lg:w-2/5 max-w-md h-full bg-cover absolute right-0 top-0"
        style="background-image: url('images/rhema-kallianpur-jbJ-_hw2yag-unsplash-2@2x.png')">
      <button class="absolute bottom-0 left-0">
        <img src="images/arrow-right (1).svg" class="px-5 py-4 bg-white" @click="++testimony"/>
      </button>
      <button class="absolute bottom-0" style="left: -56px" @click="--testimony">
        <img src="images/arrow-right (1).svg" class="px-5 transform rotate-180 py-4 bg-blue-800"/>
      </button>
    </div>
  </div>
</template>

<script>
import Testimonies from "~/components/testimonials/Testimonies"

export default {
  name: "Testimonials",
  components: { Testimonies },
  data () {
    return {
      testimony: 0
    }
  }
}
</script>

<style scoped>

</style>
