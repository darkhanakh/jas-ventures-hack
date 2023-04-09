<template>
  <div class="flex items-center justify-center px-6 py-12">
    <div>
      <div
        class="mb-6 flex h-64 max-w-sm flex-col justify-between rounded-lg border border-gray-400 bg-white px-4 py-5"
      >
        <div>
          <h4 class="mb-3 font-bold text-gray-500">{{ title }}</h4>
          <img :src="imgSrc" alt="herd" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'DroneCard',
  props: {
    title: {
      type: String,
      required: true
    },
    imgSrc: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped></style>
