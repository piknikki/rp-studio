<template>
  <div id="app">
    <nav>
      <router-link class="nav-item nav-dots" to="/">Home</router-link>
      <router-link class="nav-item nav-dots" to="/work">Work</router-link>
      <router-link class="nav-item nav-dots" to="/about">About</router-link>
      <router-link class="nav-item nav-dots" to="/contact">Contact</router-link>
    </nav>
    <h1>logo goes here</h1>
    <router-view/>
    <Home />
  </div>
</template>

<script>
import Home from '@/components/Home'

export default {
  name: 'App',
  components: {
    Home
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
