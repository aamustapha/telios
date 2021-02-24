<template>
  <div class="bg-black py-24">
    <div class="container mx-auto grid grid-cols-7 gap-4 text-white">
      <div class="col-span-2">
        <h4 class="text-2xl font-bold mb-2">
          Zetta Hotels
        </h4>
        <small class="text-gray-400 text-justify">
          Our hotel is an image of quality and profesionalism combined with hard work and precision. You can
          expect only the best services from our staff.
        </small>
        <div class="flex space-x-2 mt-4">
          <a href="#">
            <img src="images/001-facebook.svg" class="h-8 w-8"/>
          </a>
          <a href="#">
            <img src="images/002-twitter.svg" class="h-8 w-8"/>
          </a>
          <a href="#">
            <img src="images/004-google-plus.svg" class="h-8 w-8"/>
          </a>
        </div>
      </div>
      <div></div>
      <div>
        <h4 class="text-lg font-bold mb-4">
          Useful links
        </h4>
        <a href="#" class="block my-2 text-blue-800">Blog</a>
        <a href="#" class="block my-2 text-blue-800">Rooms</a>
        <a href="#" class="block my-2 text-blue-800">Gift card</a>
        <a href="#" class="block my-2 text-blue-800">Testimonials</a>
      </div>
      <div>
        <h4 class="text-lg font-bold mb-4">
          Privacy
        </h4>
        <a href="#" class="block my-2 text-blue-800">Career</a>
        <a href="#" class="block my-2 text-blue-800">About us</a>
        <a href="#" class="block my-2 text-blue-800">Contact us</a>
        <a href="#" class="block my-2 text-blue-800">Services</a>
      </div>
      <div class="col-span-2">
        <h4 class="text-lg font-bold mb-4">
          Contact info
        </h4>
        <ul class="space-y-3">
          <li> <img src="images/mail.svg" class="inline mr-2"/> example@yahoo.com</li>
          <li> <img src="images/phone.svg" class="inline mr-2"/> +0 320 422 4254</li>
          <li> <img src="images/map-pin.svg" class="inline mr-2"/> Main Str Chicago Ilinois</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer"
}
</script>

<style scoped>

</style>
