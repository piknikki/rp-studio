<template>
  <div id="app">
    <nav>
      <router-link class="nav-item nav-dots" to="/">Home</router-link>
      <router-link class="nav-item nav-dots" to="/work">Work</router-link>
      <router-link class="nav-item nav-dots" to="/about">About</router-link>
      <router-link class="nav-item nav-dots" to="/contact">Contact</router-link>
    </nav>
    <router-view/>
    <h1>logo goes here</h1>
    <Home />
    <About />
    <Work />
    <Contact />
    <Footer />
  </div>
</template>

<script>
import Home from '@/components/Home'
import About from '@/components/About'
import Work from '@/components/Work'
import Contact from '@/components/Contact'
import Footer from '@/components/Footer'

export default {
  name: 'App',
  components: {
    Home,
    About,
    Work,
    Contact,
    Footer
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: white;
  margin-top: 60px;
}

body {
  background: url("./assets/rainbowdiagonal.jpg") no-repeat center fixed;
  background-size: cover;
}
</style>
