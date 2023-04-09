<template>
  <DashboardHeader />
  <div class="drone-camera flex items-center justify-center">
    <DroneCard class="mr-10" title="Видео с первого дрона" img-src="src/assets/herd1.png" />
    <DroneCard title="Видео с второго дрона" img-src="src/assets/herd1.png" />
  </div>
  <div class="flex items-center justify-center">
    <DashboardBarChart />
  </div>
</template>
<script>
import DashboardHeader from '@/components/dashboard/DashboardHeader.vue'
import DroneCard from '@/components/dashboard/DroneCard.vue'
import DashboardBarChart from '@/components/dashboard/DashboardBarChart.vue'

export default {
  name: 'Dashboard',
  components: { DashboardBarChart, DroneCard, DashboardHeader }
}
</script>

<style scoped></style>
