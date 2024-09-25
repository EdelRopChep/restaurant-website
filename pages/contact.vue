<template>
  <div class="contact-container">
    <h1>Contact Us</h1>
    <p>If you have any questions, feel free to reach out to us!</p>

    <form @submit.prevent="submitForm">
      <div class="form-group">
        <label for="name">Name</label>
        <input
          v-model="form.name"
          type="text"
          id="name"
          placeholder="Enter your name"
        />
        <span v-if="errors.name" class="error">{{ errors.name }}</span>
      </div>

      <div class="form-group">
        <label for="email">Email</label>
        <input
          v-model="form.email"
          type="email"
          id="email"
          placeholder="Enter your email"
        />
        <span v-if="errors.email" class="error">{{ errors.email }}</span>
      </div>

      <div class="form-group">
        <label for="subject">Subject</label>
        <input
          v-model="form.subject"
          type="text"
          id="subject"
          placeholder="Enter subject"
        />
      </div>

      <div class="form-group">
        <label for="message">Message</label>
        <textarea
          v-model="form.message"
          id="message"
          rows="6"
          placeholder="Write your message here"
        ></textarea>
        <span v-if="errors.message" class="error">{{ errors.message }}</span>
      </div>

      <button type="submit" class="submit-button">Submit</button>
    </form>

    <div v-if="submitted" class="confirmation-message">
      <p>Thank you! Your message has been sent successfully.</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      form: {
        name: '',
        email: '',
        subject: '',
        message: '',
      },
      errors: {},
      submitted: false,
    };
  },
  methods: {
    validateForm() {
      this.errors = {};

      if (!this.form.name) {
        this.errors.name = 'Name is required.';
      }

      if (!this.form.email) {
        this.errors.email = 'Email is required.';
      } else if (!this.isValidEmail(this.form.email)) {
        this.errors.email = 'Valid email is required.';
      }

      if (!this.form.message) {
        this.errors.message = 'Message is required.';
      }

      return Object.keys(this.errors).length === 0;
    },
    isValidEmail(email) {
      const re = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
      return re.test(email);
    },
    submitForm() {
      if (this.validateForm()) {
        // Here you would send form data to a server or API
        this.submitted = true;

        // Reset the form after submission
        this.form = {
          name: '',
          email: '',
          subject: '',
          message: '',
        };
      }
    },
  },
};
</script>

<style scoped>
.contact-container {
  max-width: 600px;
  margin: 0 auto;
  padding: 20px;
  text-align: center;
  background-color: lemonchiffon;
}

h1 {
  margin-bottom: 20px;
}

.form-group {
  margin-bottom: 15px;
  text-align: left;
}

label {
  display: block;
  margin-bottom: 5px;
}

input,
textarea {
  width: 100%;
  padding: 10px;
  margin-bottom: 5px;
  border: 1px solid #ccc;
  border-radius: 5px;
}

.error {
  color: red;
  font-size: 12px;
}

.submit-button {
  background-color: #007bff;
  color: #fff;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.submit-button:hover {
  background-color: #0056b3;
}

.confirmation-message {
  margin-top: 20px;
  color: green;
}
</style>
