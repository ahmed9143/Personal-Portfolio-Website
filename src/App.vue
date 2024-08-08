<!-- src/App.vue -->
<template>
  <div id="app">
    <Navbar />
    <main>
      <router-view />
    </main>
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    Footer,
  },
};
</script>

<style>
body {
  font-family: 'Arial', sans-serif;
  padding-bottom: 60px;
}
main {
  min-height: 75vh;
  padding-top: 20px;
}
</style>
