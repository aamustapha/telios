<template>
  <div>
    <Banner>
      <div class=" pb-16 relative">
        <div class="max-w-screen-sm">
          <h2 class="text-6xl font-extrabold pr-3 ">Rooms</h2>
          <p>Home | Rooms</p>
        </div>
      </div>
    </Banner>
    <Rooms />

    <About></About>
    <Services/>
    <Testimonial/>
    <Restaurant/>
    <Blog/>
    <Photos/>
    <Footer/>
  </div>
</template>

<script>
import Banner from "~/components/Banner"
import About from "~/components/About"
import Services from "~/components/services/index"
import Testimonial from "~/components/testimonials/index"
import Restaurant from "~/components/restaurant/index"
import Blog from "~/components/blog/index"
import Photos from "~/components/Photos"
import Footer from "~/components/Footer"
import Rooms from "~/components/rooms/index"

export default {
  components: { Rooms, Footer, Photos, Blog, Restaurant, Testimonial, Services, About, Banner }
}
</script>
