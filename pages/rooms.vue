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
    <Rooms/>
    <Reservation/>
  </div>
</template>

<script>
import Banner from "~/components/Banner"
import Rooms from "~/components/rooms/index"
import Reservation from "~/components/Reservation"

export default {
  components: { Reservation, Rooms, Banner }
}
</script>
