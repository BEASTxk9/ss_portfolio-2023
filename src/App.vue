<template>
<Navbar></Navbar>
  <router-view/>
<Footer></Footer>
</template>

<script>
// import components
import Navbar from './components/Navbar.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'HomeView',
  components: {
    Navbar,
    Footer
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

header, section{
  min-height: 90vh;
}
</style>
