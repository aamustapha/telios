<template>
  <div class="bg-gray-light relative flex">
    <div class="container container-fluid mx-auto ">
      <div>
        <div class="max-w-2xl py-24">
          <h5 class="text-blue uppercase font-bold">
            Testimonials
          </h5>
          <h2
            class="subheading">
            We trust our customers and they trust us too
          </h2>
          <Testimonies v-model="testimony" />
        </div>
      </div>
    </div>

    <div
      class="h-full bg-cover absolute right-0 top-0"
      style="background-image: url('https://ik.imagekit.io/hooli/telios/rhema-kallianpur-jbJ-_hw2yag-unsplash-2_2x_M50RMfc8Gf.png'); width: 43%"
    >
      <button class="absolute bottom-0 left-0">
        <img alt="img" src="https://ik.imagekit.io/hooli/telios/arrow-right_-QqySiOJBG.svg" class="p-6 bg-white" @click="++testimony">
      </button>
      <button class="absolute bottom-0" style="left: -58px" @click="--testimony">
        <img alt="img" src="https://ik.imagekit.io/hooli/telios/arrow-right_-QqySiOJBG.svg" class="transform rotate-180 p-6 bg-blue">
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
      testimony: 1
    }
  }
}
</script>

<style scoped>

</style>
