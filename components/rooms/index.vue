<template>
  <div class="container container-fluid mx-auto pb-12">
    <h5 class="text-blue uppercase font-bold">
      about us
    </h5>
    <h2 class="subheading">
      Trust and quality<br/> are our atuus
    </h2>
    <div class="grid grid-cols-2 gap-6">
      <template v-for="(food, index) in menu">
        <SingleRoom :key="index" v-bind="food" />
      </template>
    </div>
  </div>
</template>

<script>
import SingleRoom from "~/components/rooms/SingleRoom"
export default {
  name: "Rooms",
  components: { SingleRoom },
  data () {
    return {
      menu: [
        {
          pic: "images/deborah-cortelazzi-gREquCUXQLI-unsplash.png",
          category: "big",
          name: "Spacious Room",
          description: "The most spacious room you will ever see in our hotel. Equipped with span and warm beds"
        },
        {
          pic: "images/christopher-jolly-GqbU78bdJFM-unsplash.png",
          category: "small",
          name: "Small Cheap Room",
          description: "Smallest and the most economic room in our hotel. Save an extra buck for your holyday"
        },
        {
          pic: "images/minh-pham-1_B4Zzh7UpQ-unsplash.png",
          category: "premium",
          name: "Big Room",
          description: "Biggest room in our hotel fully equipped with Wi-fi and hot coffee"
        },
        {
          pic: "images/sven-brandsma-GmRiN7tVW1w-unsplash.png",
          category: "expensive",
          name: "Expensive Luxury Room",
          description: "The most expensive room available for milionars and very rich people"
        },
        {
          pic: "images/deborah-cortelazzi-gREquCUXQLI-unsplash.png",
          category: "big",
          name: "Spacious Room",
          description: "The most spacious room you will ever see in our hotel. Equipped with span and warm beds"
        },
        {
          pic: "images/christopher-jolly-GqbU78bdJFM-unsplash.png",
          category: "small",
          name: "Small Cheap Room",
          description: "Smallest and the most economic room in our hotel. Save an extra buck for your holyday"
        }
      ]
    }
  }
}
</script>

<style scoped>

</style>
