<template>
  <div class="container container-fluid mx-auto py-24">
    <h5 class="text-blue uppercase font-bold">
      restaurant
    </h5>
    <h2 class="subheading">
      Explore our menu <br> and eat what you want
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
          pic: "https://ik.imagekit.io/hooli/telios/victoria-shes-UC0HZdUitWY-unsplash_2x_aFKZSMqYBi.png",
          category: "food",
          name: "Fresh fish and onions",
          description: "Fresh food directly from our restaurant ready coocked for you and you familly"
        },
        {
          pic: "https://ik.imagekit.io/hooli/telios/sheelah-brennan-UaeVmc51Ttw-unsplash_2x_jm7-95jlKiUpx.png",
          category: "desert",
          name: "Chocolate cupcakes",
          description: "Fresh food directly from our restaurant ready coocked for you and you familly"
        },
        {
          pic: "https://ik.imagekit.io/hooli/telios/sheelah-brennan-UaeVmc51Ttw-unsplash_2x_jm7-95jlKiUpx.png",
          category: "desert",
          name: "Chocolate cupcakes",
          description: "Fresh food directly from our restaurant ready coocked for you and you familly"
        },
        {
          pic: "https://ik.imagekit.io/hooli/telios/victoria-shes-UC0HZdUitWY-unsplash_2x_aFKZSMqYBi.png",
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
