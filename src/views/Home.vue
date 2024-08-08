<!-- src/views/Home.vue -->
<template>
  <div class="home text-center">
    <div class="container">
      <h1 class="display-4">Welcome to My Portfolio</h1>
      <p class="lead">
        I'm a passionate web developer with a focus on creating dynamic and responsive web applications.
      </p>
      <router-link class="btn btn-primary mt-4" to="/projects">View My Projects</router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
};
</script>

<style scoped>
.home {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background: linear-gradient(135deg, #007bff, #6610f2);
  
  color: white;
}
</style>
