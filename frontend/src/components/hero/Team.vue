<template>
  <section class="py-14">
    <div class="mx-auto max-w-screen-xl px-4 text-center md:px-8">
      <div class="mx-auto max-w-xl">
        <h3 class="text-5xl font-semibold text-white sm:text-4xl">Встречайте нашу команду</h3>
        <p class="mt-3 text-gray-600">
          Команда ShepherdVision состоит из преданных своему делу экспертов в области искусственного
          интеллекта, компьютерного зрения, беспилотной техники и управления животноводством,
          которые сотрудничают, чтобы революционизировать будущее сельского хозяйства и пастырского
          ухода.
        </p>
      </div>
      <div class="mt-12">
        <ul class="grid gap-8 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-5">
          <li v-for="(item, idx) in team" :key="idx">
            <div class="h-25 w-25 mx-auto">
              <img :src="'/assets/' + item.avatar" class="h-72 w-56 rounded-3xl" alt="" />
            </div>
            <div class="mt-2">
              <h4 class="font-semibold text-white sm:text-lg">{{ item.name }}</h4>
              <p class="text-indigo-600">{{ item.title }}</p>
            </div>
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  data() {
    return {
      team: [
        {
          avatar: 'Aza.jpg',
          name: 'Azamat Katymgali',
          title: 'Product designer'
        },
        {
          avatar: 'Edilka.jpg',
          name: 'Temirlan Yedil',
          title: 'ML engineer'
        },
        {
          avatar: 'Askar.jpg',
          name: 'Askar Nurakhmet',
          title: 'Full stack engineer'
        },
        {
          avatar: 'Temir.jpg',
          name: 'Temirlan Sartbayev',
          title: 'Data science engineer'
        },
        {
          avatar: 'Darkh.jpg',
          name: 'Darkhan Akhmetov',
          title: 'Head developer'
        }
      ]
    }
  }
}
</script>
