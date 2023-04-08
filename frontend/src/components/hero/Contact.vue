<template>
  <main class="relative py-28 bg-black">
    <div class="relative z-10 max-w-screen-xl mx-auto text-gray-600 sm:px-4 md:px-8">
      <div class="max-w-lg space-y-3 px-4 sm:mx-auto sm:text-center sm:px-0">
        <h3 class="text-cyan-400 font-semibold">Связь</h3>
        <p class="text-white text-3xl font-semibold sm:text-4xl">Свяжитесь с нами</p>
        <p class="text-gray-300">Мы бы хотели узнать ваше мнение и оценку</p>
      </div>
      <div class="mt-12 mx-auto px-4 p-8 bg-white sm:max-w-lg sm:px-8 sm:rounded-xl">
        <form @submit.prevent="onSubmit" class="space-y-5">
          <div>
            <label class="font-medium">Полное имя</label>
            <input
              type="text"
              required
              class="w-full mt-2 px-3 py-2 text-gray-500 bg-transparent outline-none border focus:border-gray-800 shadow-sm rounded-lg"
            />
          </div>
          <div>
            <label class="font-medium">Email</label>
            <input
              type="email"
              required
              class="w-full mt-2 px-3 py-2 text-gray-500 bg-transparent outline-none border focus:border-gray-800 shadow-sm rounded-lg"
            />
          </div>
          <div>
            <label class="font-medium">Номер телефона</label>
            <div class="relative mt-2">
              <div class="absolute inset-y-0 left-3 my-auto h-6 flex items-center border-r pr-2">
                <select class="text-sm bg-transparent outline-none rounded-lg h-full">
                  <option>KZ</option>
                  <option>AZ</option>
                  <option>US</option>
                </select>
              </div>
              <input
                type="number"
                placeholder="+7 (700) 7777777"
                required
                class="w-full pl-[4.5rem] pr-3 py-2 appearance-none bg-transparent outline-none border focus:border-gray-800 shadow-sm rounded-lg"
              />
            </div>
          </div>
          <div>
            <label class="font-medium">Сообщение</label>
            <textarea
              required
              class="w-full mt-2 h-36 px-3 py-2 resize-none appearance-none bg-transparent outline-none border focus:border-gray-800 shadow-sm rounded-lg"
            ></textarea>
          </div>
          <button class="w-full px-4 py-2 text-white font-medium bg-gray-800 hover:bg-gray-700 active:bg-gray-900 rounded-lg duration-150">Отправить</button>
        </form>
      </div>
    </div>
    <div
      class="absolute inset-0 blur-[118px] max-w-lg h-[800px] mx-auto sm:max-w-3xl sm:h-[400px]"
      :style="{
        background: 'linear-gradient(106.89deg, rgba(150, 90, 210, 0.1) 15.73%, rgba(10, 130, 200, 0.3) 15.74%, rgba(120, 40, 120, 0.2) 56.49%, rgba(50, 40, 180, 0.5) 115.91%)',
}"
></div>

  </main>
</template>
<script>
export default {
  methods: {
    onSubmit() {
      // Handle form submission logic
    },
  },
};
</script>
<style scoped>
  /* Add any styles for the component here */
</style>