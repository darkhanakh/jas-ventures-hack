<template>
  <!-- Navbar -->
  <nav
    class="z-10 flex w-full items-center bg-black p-4 md:flex-row md:flex-nowrap md:justify-start"
  >
    <div
      class="mx-autp flex w-full flex-wrap items-center justify-between px-4 md:flex-nowrap md:px-10"
    >
      <router-link to="/">
        <img src="@/assets/back-button-svgrepo-com.svg" alt="" class="mr-3 h-6" />
      </router-link>
      <!-- Brand -->
      <a class="= hidden text-2xl font-semibold text-white lg:inline-block" href=""> Аналитика </a>
      <!-- Form -->
      <form class="mr-3 hidden flex-row flex-wrap items-center md:flex lg:ml-auto">
        <div class="relative flex w-full flex-wrap items-stretch">
          <span
            class="text-blueGray-300 absolute absolute z-10 h-full w-8 items-center justify-center rounded bg-transparent py-3 pl-3 text-center text-base font-normal leading-snug"
          >
            <img src="@/assets/icons8-search.svg" alt="search icon" />
          </span>
          <input
            type="text"
            placeholder="Поиск"
            class="placeholder-blueGray-300 text-blueGray-600 relative w-full rounded border-0 bg-white bg-white px-3 py-3 pl-10 text-sm shadow outline-none focus:outline-none focus:ring"
          />
        </div>
      </form>
      <!-- User -->
    </div>
  </nav>
  <!-- End Navbar -->
</template>

<script></script>
