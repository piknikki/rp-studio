<template>
  <div id="app">
    <nav class="navbar" role="navigation">
      <div class="navbar-brand" to="/">
<!--        image logo goes here -->
<!--        <img class="d-inline-block mylogo" alt="my logo" src="./assets/logo.png">-->
        <span class="align-content-center myname">vera petersen</span>
      </div>

      <div class="navbar-menu">
        <div class="navbar-end is-active">
          <router-link class="nav-item nav-dots" to="/">Home</router-link>
          <router-link class="nav-item nav-dots" to="/work">Work</router-link>
          <router-link class="nav-item nav-dots" to="/about">About</router-link>
          <router-link class="nav-item nav-dots" to="/contact">Contact</router-link>
        </div>
      </div>
    </nav>
    <router-view/>
    <About />
    <Work />
    <Contact />
    <Footer />
  </div>
</template>

<script>
// import Home from '@/components/Home'
import About from '@/components/About'
import Work from '@/components/Work'
import Contact from '@/components/Contact'
import Footer from '@/components/Footer'

export default {
  name: 'App',
  components: {
    // Home,
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

#nav {
  padding: 30px;
  cursor: pointer;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}

.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-size: 1.5em;
  padding: 10px 100px;
}

.nav-item {
  padding: 10px;
}

.nav-dots {
  color: lightpink;
  font-size: 1.5em;
  letter-spacing: 1px;
  vertical-align: center;
  margin-left: 1px;
  margin-right: 6px;
  border-radius: 20px;
}

.nav-dots:hover {
  border-left: 1px dotted deeppink;
  border-right: 1px dotted deeppink;
  margin-left: 0;
  margin-right: 5px;
  color: deeppink;
  border-radius: 20px;
  text-decoration: none;
}
</style>
