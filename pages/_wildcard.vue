<template>
  <div>
    <Banner class="mb-12">
      <div class=" pb-16 relative">
        <div class="max-w-screen-sm">
          <h2 class="page-title">
            Page not found
          </h2>
          <p>Home | 404</p>
        </div>
      </div>
    </Banner>
    <div class="container mx-auto my-12">
      You already know what this means. Go back to <router-link to="/" class="text-blue">
        Home
      </router-link>,
      <router-link to="/rooms" class="text-blue">
        Rooms
      </router-link> or
      <router-link to="/about-us" class="text-blue">
        About
      </router-link>.
    </div>
  </div>
</template>

<script>
export default {
  name: "Wildcard"
}
</script>

<style scoped>

</style>
