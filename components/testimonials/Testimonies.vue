<template>
  <div class="testimony">
    <template v-for="(testimony, index) in testimonies">
      <Testimony v-bind="testimony" v-if="index === Math.abs(value % testimonies.length)" :key="index"/>
    </template>
    <ul class="flex mt-8 space-x-1">
      <template v-for="(testimony, index) in testimonies">
        <li
            class="inline-block w-3 h-3 rounded-full bg-gray"
            :key="index"
            v-bind="isActive(index)"
            @click="select(index)"></li>
      </template>
    </ul>
  </div>
</template>

<script>
import Testimony from "~/components/testimonials/Testimony"

export default {
  name: "Testimonies",
  components: { Testimony },
  props: { value: { type: Number, default: 0 } },
  data () {
    return {
      testimonies: [
        {
          name: "John Doe",
          role: "IT Engineer",
          pic: "images/marius-ciocirlan-vMV6r4VRhJ8-unsplash.png",
          testimony: "I'm very glad I had the opportunity to visit this hotel. The stuff is very friendly and I will definetly visit the hotel again next year."
        },
        {
          name: "Usman Doe",
          role: "IT Engineer",
          pic: "images/marius-ciocirlan-vMV6r4VRhJ8-unsplash.png",
          testimony: "I'm very glad I had the opportunity to visit this hotel. The stuff is very friendly and I will definetly visit the hotel again next year."
        },
        {
          name: "John Irale",
          role: "IT Engineer",
          pic: "images/marius-ciocirlan-vMV6r4VRhJ8-unsplash.png",
          testimony: "I'm very glad I had the opportunity to visit this hotel. The stuff is very friendly and I will definetly visit the hotel again next year."
        },
        {
          name: "Sophie Doe",
          role: "IT Engineer",
          pic: "images/marius-ciocirlan-vMV6r4VRhJ8-unsplash.png",
          testimony: "I'm very glad I had the opportunity to visit this hotel. The stuff is very friendly and I will definetly visit the hotel again next year."
        }
      ]
    }
  },
  computed: {
    isActive () {
      return (index) => {
        if (index === Math.abs(this.value % this.testimonies.length)) {
          return {
            class: "bg-blue"
          }
        }
        return {}
      }
    }
  },
  methods: {
    select (index) {
      this.$emit("input", index)
    }
  }

}
</script>

<style scoped>
</style>
