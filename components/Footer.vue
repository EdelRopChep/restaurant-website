<template>
  <footer class="footer">
    <div class="container">
      <p>© 2024 MyCompany. All rights reserved.</p>
      <div class="social-links">
        <a href="https://twitter.com" target="_blank" class="social-icon">Twitter</a>
        <a href="https://facebook.com" target="_blank" class="social-icon">Facebook</a>
        
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style scoped>
.footer {
  background-color: rebeccapurple;
  color: white;
  padding: 1.5rem 0;
  text-align: center;
}

.footer p {
  margin: 0;
}

.footer .social-links {
  margin-top: 1rem;
}

.footer .social-links .social-icon {
  color: white;
  margin: 0 0.5rem;
  text-decoration: none;
}

.footer .social-links .social-icon:hover {
  color: #ddd;
}
</style>
