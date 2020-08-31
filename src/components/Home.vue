<template>
  <div>
    <h2>Welcome to Red Panda Studio. I am Vera Petersen and this is my work.</h2>
    <About />
    <Work />
    <Contact />
    <Footer />
  </div>
</template>

<script>
import About from '@/components/About'
import Work from '@/components/Work'
import Contact from '@/components/Contact'
import Footer from '@/components/Footer'

export default {
  name: 'home',
  components: {
    About,
    Work,
    Contact,
    Footer
  }
}
</script>

<style scoped>

</style>
