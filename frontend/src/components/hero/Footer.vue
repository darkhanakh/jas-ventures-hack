<template>
  <footer class="mx-auto max-w-screen-xl bg-black px-4 py-5 text-white md:px-8">
    <div class="max-w-lg sm:mx-auto sm:text-center">
      <img src="@/assets/logo1.jpg" class="w-32 sm:mx-auto" />
      <p class="mt-2 text-[15px] leading-relaxed">
        Расширение возможностей фермеров и владельцев скота с помощью передовых беспилотных
        технологий, основанных на искусственном интеллекте, для мониторинга, защиты и более
        эффективного и устойчивого управления стадами. Общайтесь с нами в социальных сетях и
        подписывайтесь на наш информационный бюллетень, чтобы получать самые последние обновления и
        информацию.
      </p>
    </div>
    <ul class="mt-8 items-center justify-center space-y-5 sm:flex sm:space-x-4 sm:space-y-0">
      <li v-for="(item, index) in footerLinks" :key="index">
        <a
          :href="item.url"
          class="text-[15px] font-semibold hover:text-gray-900"
          target="_blank"
          rel="noopener noreferrer"
        >
          {{ item.title }}
        </a>
      </li>
    </ul>
  </footer>
</template>
<script>
export default {
  data() {
    return {
      footerLinks: [
        { title: 'Меню', url: 'https://www.example.com' },
        { title: 'Про нас', url: 'https://www.example.com/about' },
        { title: 'Сервисы', url: 'https://www.example.com/services' },
        { title: 'Контакты', url: 'https://www.example.com/contact' }
      ]
    }
  }
}
</script>
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700&display=swap');

body {
  font-family: 'Roboto', sans-serif;
}
</style>
