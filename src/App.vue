<template>
  <Navbar />
  <Welcome />
  <About />
  <Portfolio />
</template>

<script>
  import Navbar from './components/Navbar.vue';
  import Welcome from './components/Welcome.vue';
  import About from './components/About.vue';
  import Portfolio from './components/Portfolio.vue';
  

  export default {
    components: {
      Navbar,
      Welcome,
      About,
      Portfolio
    }
  }
</script>