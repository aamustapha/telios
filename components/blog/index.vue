<template>
  <div class="container container-fluid pb-24 pt-12">
    <h5 class="text-blue uppercase font-bold">
      blog
    </h5>
    <h2 class="font-black text-big mt-2 mb-4 max-w-xl">
      Read our newest blog <br>post right away
    </h2>

    <div class="grid grid-cols-3 gap-3">
      <SingleArticle v-for="(article, index) in articles" :key="index" v-bind="article" />
    </div>
  </div>
</template>

<script>
import SingleArticle from "~/components/blog/SingleArticle"

export default {
  name: "Blog",
  components: { SingleArticle },
  data () {
    return {
      articles: [
        {
          pic: "https://ik.imagekit.io/hooli/telios/vicky-sim-mj51pZwan9c-unsplash-1_sw2lJvPML.png",
          category: "food and life",
          title: "Succed in hotel business",
          summary: "Fresh food directly from our restaurant ready coocked for you"
        },
        {
          pic: "https://ik.imagekit.io/hooli/telios/victoria-shes-UC0HZdUitWY-unsplash-2_2x_8671MgOKJIC8.png",
          category: "cooking",
          title: "Cooking delicious food",
          summary: "Fresh food directly from our restaurant ready coocked for you"
        },
        {
          pic: "https://ik.imagekit.io/hooli/telios/sheelah-brennan-UaeVmc51Ttw-unsplash-2_2x_KNEsqnS-8u.png",
          category: "fruits",
          title: "Getting fresh fruits",
          summary: "Fresh food directly from our restaurant ready coocked for you"
        }, {
          pic: "https://ik.imagekit.io/hooli/telios/sheelah-brennan-UaeVmc51Ttw-unsplash-2_2x_KNEsqnS-8u.png",
          category: "fruits",
          title: "Getting fresh fruits",
          summary: "Fresh food directly from our restaurant ready coocked for you"
        },
        {
          pic: "https://ik.imagekit.io/hooli/telios/victoria-shes-UC0HZdUitWY-unsplash-2_2x_8671MgOKJIC8.png",
          category: "cooking",
          title: "Cooking delicious food",
          summary: "Fresh food directly from our restaurant ready coocked for you"
        },
        {
          pic: "https://ik.imagekit.io/hooli/telios/vicky-sim-mj51pZwan9c-unsplash-1_sw2lJvPML.png",
          category: "food and life",
          title: "Succed in hotel business",
          summary: "Fresh food directly from our restaurant ready coocked for you and you familly"
        }
      ]
    }
  }
}
</script>

<style scoped>

</style>
