<!-- src/components/Footer.vue -->
<template>
  <footer class="bg-dark text-white text-center py-3 mt-5">
    <div class="container">
      <p>&copy; 2024 My Portfolio. All rights reserved.</p>
      <p>
        Follow me on
        <a class="text-white" href="https://github.com/ahmed9143" target="_blank">GitHub</a> |
        <a class="text-white" href="https://www.linkedin.com/in/ahmed-elsayed-a064071bb/" target="_blank">LinkedIn</a>
      </p>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
footer {
  position: relative;
  bottom: 0;
  width: 100%;
}
a {
  text-decoration: none;
}
a:hover {
  text-decoration: underline;
}
</style>
