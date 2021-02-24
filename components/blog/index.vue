<template>
  <div class="container mx-auto pb-24 pt-12">
    <h5 class="text-blue uppercase font-bold">
      blog
    </h5>
    <h2 class="font-black text-4xl mt-2 mb-4 max-w-lg">
      Read our newest blog post right away
    </h2>

    <div class="grid grid-cols-3 gap-8">
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
          pic: "images/vicky-sim-mj51pZwan9c-unsplash-1.png",
          category: "food and life",
          title: "Succed in hotel business",
          summary: "Fresh food directly from our restaurant ready coocked for you and you familly"
        },
        {
          pic: "images/victoria-shes-UC0HZdUitWY-unsplash-2@2x.png",
          category: "cooking",
          title: "Cooking delicious food",
          summary: "Fresh food directly from our restaurant ready coocked for you and you familly"
        },
        {
          pic: "images/sheelah-brennan-UaeVmc51Ttw-unsplash-1@2x.png",
          category: "fruits",
          title: "Getting fresh fruits",
          summary: "Fresh food directly from our restaurant ready coocked for you and you familly"
        }, {
          pic: "images/sheelah-brennan-UaeVmc51Ttw-unsplash-1@2x.png",
          category: "fruits",
          title: "Getting fresh fruits",
          summary: "Fresh food directly from our restaurant ready coocked for you and you familly"
        },
        {
          pic: "images/victoria-shes-UC0HZdUitWY-unsplash-2@2x.png",
          category: "cooking",
          title: "Cooking delicious food",
          summary: "Fresh food directly from our restaurant ready coocked for you and you familly"
        },
        {
          pic: "images/vicky-sim-mj51pZwan9c-unsplash-1.png",
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
