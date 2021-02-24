<template>
  <div>
    <Banner>
      <div class=" pb-48 relative">
        <div class="max-w-screen-sm">
          <h2 class="text-6xl font-black ">The best hotel you will ever need</h2>
          <summary>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
            dolore
            magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
            commodo
            consequat.
          </summary>
        </div>

        <div class="py-8 absolute container mt-24 text-black">
          <div class="flex justify-end">
            <button>
              <img src="images/arrow-right (1).svg" class="px-5 py-4 transform rotate-180 bg-white" />
            </button>
            <button>
              <img src="images/arrow-right (1).svg" class="px-5 py-4 bg-blue-800"/>
            </button>
          </div>
          <div class="bg-white py-8 px-12 shadow-lg flex justify-between items-end">
            <div class="w-11/12 grid grid-cols-3 gap-4">
              <TInput type="text" label="Check-in date" placeholder="check in date"/>
              <TInput type="text" label="Checkout date" placeholder="check out date"/>
              <TInput type="text" label="Rooms" placeholder="rooms"/>
            </div>
            <button class="bg-blue-800 h-12 w-12 mb-4">
              <img src="images/send.svg" class="d-block mx-auto" />
            </button>
          </div>
        </div>
      </div>
    </Banner>
    <About></About>
    <Services />
    <Testimonial />
    <Restaurant />
    <Blog />
    <Photos />
    <Footer />
  </div>
</template>

<script>
import Banner from "~/components/Banner"
import TInput from "~/components/TInput"
import About from "~/components/About"
import Services from "~/components/services/index"
import Testimonial from "~/components/testimonials/index"
import Restaurant from "~/components/restaurant/index"
import Blog from "~/components/blog/index"
import Photos from "~/components/Photos"
import Footer from "~/components/Footer"

export default {
  components: { Footer, Photos, Blog, Restaurant, Testimonial, Services, About, TInput, Banner }
}
</script>

<style>
* {
  font-family: 'Poppins', sans-serif;
}
</style>
