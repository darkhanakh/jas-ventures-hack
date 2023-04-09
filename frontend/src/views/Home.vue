<template>
  <div class="bg-black">
    <TheHeader />
    <HeroMain />
    <Features />
    <Team />
    <Contact />
    <Footer />
  </div>
</template>

<script>
import TheHeader from '@/components/hero/TheHeader.vue'
import HeroMain from '@/components/hero/HeroMain.vue'
import Features from '@/components/hero/Features.vue'
import Team from '@/components/hero/Team.vue'
import Contact from '@/components/hero/Contact.vue'
import Footer from '@/components/hero/Footer.vue'

export default {
  components: {
    TheHeader,
    HeroMain,
    Features,
    Team,
    Contact,
    Footer
  }
}
</script>
