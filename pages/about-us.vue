<template>
  <div>
    <Banner class="mb-12">
      <div class=" pb-16 relative">
        <div class="max-w-screen-sm">
          <h2 class="text-6xl font-extrabold pr-3 ">
            About Us
          </h2>
          <p>Home | About Us</p>
        </div>
      </div>
    </Banner>
    <About />
    <Services />
    <Testimonials />
    <TSpacer class="my-12" />
  </div>
</template>

<script>
import Banner from "~/components/Banner"
import About from "~/components/About"
import Services from "~/components/services/index"
import Testimonials from "~/components/testimonials/index"
import TSpacer from "~/components/Spacer"
export default {
  components: { TSpacer, Testimonials, Services, About, Banner }
}
</script>

<style scoped>

</style>
