<template>
  <div class="container container-fluid mx-auto py-24">
    <h5 class="text-blue uppercase font-bold">
      restaurant
    </h5>
    <h2 class="font-extrabold text-big mt-2 mb-4 max-w-xl">
      Explore our menu and eat what you want
    </h2>
    <div class="grid grid-cols-2 gap-4">
      <template v-for="(food, index) in menu">
        <FoodMenu :key="index" v-bind="food" />
      </template>
    </div>
  </div>
</template>

<script>
import FoodMenu from "~/components/restaurant/FoodMenu"
export default {
  name: "Restaurant",
  components: { FoodMenu },
  data () {
    return {
      menu: [
        {
          pic: "images/victoria-shes-UC0HZdUitWY-unsplash@2x.png",
          category: "food",
          name: "Fresh fish and onions",
          description: "Fresh food directly from our restaurant ready coocked for you and you familly"
        },
        {
          pic: "images/sheelah-brennan-UaeVmc51Ttw-unsplash@2x.png",
          category: "desert",
          name: "Chocolate cupcakes",
          description: "Fresh food directly from our restaurant ready coocked for you and you familly"
        },
        {
          pic: "images/sheelah-brennan-UaeVmc51Ttw-unsplash@2x.png",
          category: "desert",
          name: "Chocolate cupcakes",
          description: "Fresh food directly from our restaurant ready coocked for you and you familly"
        },
        {
          pic: "images/victoria-shes-UC0HZdUitWY-unsplash@2x.png",
          category: "food",
          name: "Fresh fish and onions",
          description: "Fresh food directly from our restaurant ready coocked for you and you familly"
        }
      ]
    }
  }
}
</script>

<style scoped>

</style>
