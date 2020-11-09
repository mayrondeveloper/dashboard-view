<template>
  <div id="app">
      <sidenav />
      <Dashboard />
  </div>
</template>

<script>
import Dashboard from './components/dashboard.vue'
import Sidenav from "@/components/sidenav";

export default {
  name: 'App',
  data() {
    return {
      menuOpen: false
    }
  },
  components: {
    Sidenav,
    Dashboard
  }
}
</script>

<style lang="scss">
body {
  padding: 0;
  margin: 0;
}

h1 {
  padding: 0;
  margin: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin: 0;
  padding: 0;
  display: flex;
  background: #FAFBFC;
}
</style>
