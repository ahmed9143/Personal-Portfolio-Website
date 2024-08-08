<!-- src/views/About.vue -->
<template>
  <div class="about container mt-5 pb-5">
    <h2 class="mb-4 text-center">About Me</h2>
    <div class="row align-items-center">
      <div class="col-md-6">
        <p>
          I'm a Frontend developer with experience in building web applications using modern technologies like Vue.js and Bootstrap. My passion is to create user-friendly, scalable, and efficient web solutions.
        </p>
      </div>
      <div class="col-md-6 text-center">
        <img src="https://via.placeholder.com/150" alt="Profile Picture" class="rounded-circle img-fluid" />
      </div>
    </div>
    <h3 class="mt-5 text-center">Skills</h3>
    <div class="row mt-4 text-center">
      <div class="col-md-4">
        <h5 class="mb-3">Frontend</h5>
        <ul>
          <li>HTML5</li>
          <li>CSS3</li>
          <li>JavaScript (ES6+)</li>
          <li>Vue.js</li>
          <li>Bootstrap</li>
        </ul>
      </div>
      <div class="col-md-4">
        <h5 class="mb-3">Backend</h5>
        <ul>
          <li>Node.js **</li>
          <li>Express.js **</li>
          <li>RESTful APIs **</li>
        </ul>
      </div>
      <div class="col-md-4">
        <h5 class="mb-3">Tools</h5>
        <ul>
          <li>Git & GitHub</li>
          <li>Webpack</li>
          <li>Vite</li>
          <li>Yarn</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "About",
};
</script>

<style scoped>
.about {
  background-color: #f8f9fa;
  border-radius: 10px;
  padding: 30px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

h2 {
  color: #007bff;
  font-weight: bold;
}

h3 {
  color: #343a40;
  font-weight: bold;
}

h5 {
  color: #007bff;
  font-weight: bold;
}

ul {
  list-style-type: none;
  padding: 0;
}

ul li::before {
  content: "•";
  color: #007bff;
  display: inline-block;
  width: 1em;
  margin-left: -1em;
}

ul li {
  font-size: 1.1rem;
  margin-bottom: 8px;
}

p {
  font-size: 1.2rem;
  color: #343a40;
}

img {
  max-width: 150px;
  border: 4px solid #007bff;
}
</style>
