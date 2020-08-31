<template>
  <div id="app">
    <nav class="navbar" role="navigation">
      <div class="navbar-brand" to="/">
<!--        image logo goes here -->
<!--        <img class="d-inline-block mylogo" alt="my logo" src="./assets/logo.png">-->
        <span class="align-content-center myname">vera petersen</span>
      </div>

      <div class="navbar-menu">
        <div class="navbar-end">
          <router-link class="nav-item nav-dots" to="/">Home</router-link>
          <router-link class="nav-item nav-dots" to="/work">Work</router-link>
          <router-link class="nav-item nav-dots" to="/about">About</router-link>
          <router-link class="nav-item nav-dots" to="/contact">Contact</router-link>
        </div>
      </div>
    </nav>
    <router-view/>
  </div>
</template>

<script>
// import Home from '@/components/Home'

export default {
  name: 'App'
}
</script>

<style lang="scss">
* {
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: white;
  margin-top: 60px;
  margin-left: auto;
  margin-right: auto;
  width: 80%;
}

body {
  background: url("./assets/rainbowdiagonal.jpg") no-repeat center fixed;
  background-size: cover;
}

#nav {
  padding: 30px;
  cursor: pointer;
}

.navbar {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  font-size: 1.5em;
  padding: 20px;
}

.navbar-brand {
  justify-content: flex-start;
}

.navbar-menu {
  display: flex;
}

.navbar-end {
  justify-content: flex-end;
}

.navbar a {
  padding: 2px 10px;
}

.nav-dots {
  color: deeppink;
  text-decoration: none;
  font-size: 1em;
  letter-spacing: 1px;
  vertical-align: center;
  //margin-left: 1px;
  //margin-right: 6px;
  border-radius: 20px;
  border-bottom: lightpink solid 2px;
  margin: 0 10px;
}

.nav-dots:hover {
  //border-left: 1px dotted deeppink;
  //border-right: 1px dotted deeppink;
  //margin-left: 0;
  //margin-right: 5px;
  //color: deeppink;
  background-color: lightpink;
  border-radius: 20px;
  text-decoration: none;
}
</style>
