<template>
  <div>
    <Banner>
      <div class="pb-48 relative">
        <div class="pt-4">
          <h2 class="text-verybig font-black leading-loose mb-6 pt-16 ">
            The best hotel <br> you will ever need
          </h2>
          <p class="text-base">
            Lorem ipsum dolor sit amet, consectetur <br>
            adipiscing elit, sed do eiusmod tempor incididunt <br>
            ut labore et dolore magna aliqua. Ut enim ad
          </p>
        </div>

        <div class="py-8 absolute px-1 container mt-16 text-black">
          <div class="flex justify-end">
            <button>
              <img src="https://ik.imagekit.io/hooli/telios/arrow-right_-QqySiOJBG.svg" class="px-4 py-4 transform rotate-180 bg-white">
            </button>
            <button>
              <img src="https://ik.imagekit.io/hooli/telios/arrow-right_-QqySiOJBG.svg" class="px-4 py-4 bg-blue">
            </button>
          </div>
          <div class="bg-white py-6 pb-12 px-24 shadow-xl flex justify-between items-end">
            <div class="flex gap-3 items-end text-medium w-full">
              <TInput type="text" label="Check In Date" placeholder="check in date" input-class="bg-gray-semilight border-gray-semilight text-gray-semidark" c;a/>
              <TInput type="text" label="Check Out Date" placeholder="check out date" input-class="bg-gray-semilight border-gray-semilight text-gray-semidark" />
              <TInput type="text" label="Rooms" placeholder="rooms" input-class="bg-gray-semilight border-gray-semilight text-gray-semidark" />
              <button class="bg-blue h-12 w-12 mb-4 flex-shrink-0">
                <img src="https://ik.imagekit.io/hooli/telios/send_1v6H9jZIyghJ.svg" class="d-block mx-auto">
              </button>
            </div>
          </div>
        </div>
      </div>
    </Banner>
    <TSpacer class="mb-30" />
    <About />
    <Services />
    <Testimonial />
    <Restaurant />
    <Blog />
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
import TSpacer from "~/components/Spacer"

export default {
  components: { TSpacer, Blog, Restaurant, Testimonial, Services, About, TInput, Banner }
}
</script>
