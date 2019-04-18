<template lang="pug">
#app
  .navbar.navbar-expand-lg.navbar-dark
    a.navbar-brand.text-light Example
    button.navbar-toggler( type="button" data-toggle="collapse" data-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation")
      span.navbar-toggler-icon 
    .collapse.navbar-collapse#navbarNavAltMarkup
      .navbar-nav
        router-link.nav-item.nav-link(to="/") Home
        router-link.nav-item.nav-link(to="/About") About
  .container-fluid
    router-view
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue"

export default {
  name: "app",
  components: {
    HelloWorld
  }
}
</script>

<style lang="scss">
body {
  background-color: #f6f6f6;
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.navbar {
  background-color: #35495e;
}
</style>
