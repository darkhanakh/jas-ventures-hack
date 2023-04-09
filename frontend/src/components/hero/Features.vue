<template>
  <section class="custom-screen py-20 text-gray-600">
    <div class="mx-auto max-w-xl text-center">
      <h2 class="mb-3.5 text-4xl font-semibold text-white sm:text-4xl">
        Преимущества использования нашей технологии
      </h2>
      <p class="mt-3 text-gray-400">
        Наша технология обеспечивает максимальную продуктивность, экономию времени и денег, а также
        повышение качества жизни животных на вашей ферме.
      </p>
    </div>
    <div class="mx-auto mt-12 max-w-7xl ">
      <ul class="flex justify-between align-middle">
        <li v-for="(item, idx) in featuresList" :key="idx">
          <a 
            :href="item.href"
            target="_blank"
            class="card group mr-5 block h-60 max-w-2xl space-y-3 rounded-lg border from-gray-50 to-gray-100 p-4 hover:bg-white sm:p-6"
          >
            <h2
              class="flex items-center gap-x-0 text-xl font-semibold text-white duration-200 group-hover:gap-x-3"
            >
              {{ item.title }}
            </h2>
            <p>
              {{ item.desc }}</p>
          </a>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      featuresList: [
        {
          title: 'Максимизируйте свою прибыль',
          desc: 'Наша технология на основе дронов и компьютерного зрения помогает фермерам максимизировать прибыльность бизнеса, оптимизируя использование пастбищ, управляя запасами кормов и предотвращая потери животных.'
        },
        {
          title: 'Автоматизация управления стадом',
          desc: 'Использование дрона с ИИ облегчает процесс управления стадом, освобождая время пастухов и владельцев скота для выполнения других задач или даже снижая необходимость в пастухе вовсе'
        },
        {
          title: 'Снижение потерь скота',
          desc: 'ShepherdVision помогает отслеживать отделившихся животных и возвращает их к основному стаду, что снижает риск потери скота из-за хищников или других опасностей.'
        }
      ],
      hoveredIndex: null,
    }
  },

  methods: {
    handleHover(idx) {
      this.hoveredIndex = idx
    },
    handleLeave() {
      this.hoveredIndex = null
    }
  }
}
</script>

<style>
  .card:hover h2 {
    @apply text-black;
  }
  .card:hover p{
    @apply text-black font-semibold;
  }
</style>