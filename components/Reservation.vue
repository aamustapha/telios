<template>
  <div class="bg-gray-light my-12">
    <div class=" container mx-auto py-12 text-black">
      <div class="py-8 px-12 flex justify-between ">
        <div class="grid grid-cols-4 gap-4 items-end">
          <TInput type="text" label="Check-in date" placeholder="check in date" input-class="bg-white border-gray" />
          <TInput type="text" label="Checkout date" placeholder="check out date" input-class="bg-white border-gray" />
          <TInput type="text" label="Rooms" placeholder="rooms" input-class="bg-white border-gray" />
          <button class="bg-blue mb-3 text-white h-12">
            Submit
            <img src="https://ik.imagekit.io/hooli/telios/send_1v6H9jZIyghJ.svg" alt="send" class="ml-2 inline-block">
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import TInput from "~/components/TInput"
export default {
  name: "Reservation",
  components: { TInput }
}
</script>

<style scoped>

</style>
