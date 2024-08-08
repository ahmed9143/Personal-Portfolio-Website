<!-- src/views/Projects.vue -->
<template>
  <div class="projects container mt-5">
    <h2 class="mb-4 text-center">My Projects</h2>
    <div class="row">
      <div class="col-md-6 col-lg-4 mb-4" v-for="project in projects" :key="project.id">
        <div class="card h-100">
          <img :src="project.image" class="card-img-top" :alt="project.name" />
          <div class="card-body">
            <h5 class="card-title">{{ project.name }}</h5>
            <p class="card-text">{{ project.description }}</p>
          </div>
          <div class="card-footer">
            <a :href="project.link" class="btn btn-primary btn-block" target="_blank">View Project</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Projects",
  data() {
    return {
      projects: [
        {
          id: 1,
          name: "Portfolio Website",
          description: "A personal portfolio website built with Vue.js and Bootstrap.",
          image: "https://via.placeholder.com/400x200.png?text=Project+One",
          link: "https://github.com/your-username/portfolio-website",
        },
        {
          id: 2,
          name: "Graduation Projects Management System",
          description: "System Designed to manage projects for the final yearn university students.",
          image: "https://via.placeholder.com/400x200.png?text=Project+Two",
          link: "https://github.com/Abdelrahman61923/graduation-platform.git",
        },
        {
          id: 3,
          name: "E-commerce Platform",
          description: "An e-commerce platform built with Vue.js and Node.js.",
          image: "https://via.placeholder.com/400x200.png?text=Project+Two",
          link: "https://github.com/your-username/ecommerce-platform",
        },

        // Add more projects here
      ],
    };
  },
};
</script>

<style scoped>
.projects {
  text-align: center;
}
.card {
  transition: transform 0.3s ease-in-out;
}
.card:hover {
  transform: scale(1.05);
}
.card-title {
  color: #007bff;
}
.card-footer {
  background: white;
}
.btn-block {
  width: 100%;
}
</style>
