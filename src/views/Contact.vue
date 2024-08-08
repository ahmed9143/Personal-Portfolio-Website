<!-- src/views/Contact.vue -->
<template>
  <div class="contact container mt-5">
    <h2 class="mb-4 text-center">Contact Me</h2>
    <form @submit.prevent="sendMessage">
      <div class="mb-3">
        <label for="name" class="form-label">Name</label>
        <input type="text" class="form-control shadow-none" id="name" v-model="form.name" required />
      </div>
      <div class="mb-3">
        <label for="email" class="form-label">Email</label>
        <input type="email" class="form-control shadow-none" id="email" v-model="form.email" required />
      </div>
      <div class="mb-3">
        <label for="message" class="form-label">Message</label>
        <textarea class="form-control shadow-none" id="message" rows="5" v-model="form.message" required></textarea>
      </div>
      <button type="submit" class="btn btn-primary btn-block">Send Message</button>
    </form>
  </div>
</template>

<script>
export default {
  name: "Contact",
  data() {
    return {
      form: {
        name: "",
        email: "",
        message: "",
      },
    };
  },
  methods: {
    sendMessage() {
      alert(`Message sent by ${this.form.name}!`);
      this.form = { name: "", email: "", message: "" }; // Reset form
    },
  },
};
</script>

<style scoped>
.contact {
  max-width: 600px;
  margin: auto;
}
.form-label {
  font-weight: bold;
}
.btn-block {
  width: 100%;
}
</style>
