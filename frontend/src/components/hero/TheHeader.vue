<template>
  <header class="absolute inset-x-0 top-0 z-50">
    <nav
      class="container mx-auto flex items-center justify-between p-6 lg:px-8"
      aria-label="Global"
    >
      <div class="flex lg:flex-1">
        <a href="#" class="-m-1.5 p-1.5">
          <img class="h-32 w-auto" src="@/assets/logo1.jpg" alt="site logo" />
        </a>
      </div>
      <div class="lg:flex lg:flex-1 lg:justify-center">
        <p class="rounded-full text-lg font-semibold leading-6 text-white"></p>
      </div>
      <div class="hidden lg:flex lg:flex-1 lg:justify-end">
        <router-link class="rounded-full text-lg font-semibold leading-6 text-white" to="/"
          >ShepherdVision
        </router-link>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style scoped></style>
