<template>
  <nav class="navbar">
    <div class="container">
      <!-- Search Bar (Left) -->
      <div class="navbar-right">
        <input
          type="text"
          placeholder="Search..."
          class="search-bar"
        />
      </div>

      <!-- Collapsible Tab (Center) -->
      <div class="navbar-center">
        <button class="toggle-button" @click="toggleMenu">
        MENU
        </button>
        <div v-if="isMenuOpen" class="collapsing-menu">
          <NuxtLink to="/" class="navbar-item">Home</NuxtLink>
          <NuxtLink to="/about" class="navbar-item">About</NuxtLink>
          <NuxtLink to="/menu" class="navbar-item">Menu</NuxtLink>
          <NuxtLink to="/contact" class="navbar-item">Contact</NuxtLink>
        </div>
      </div>

      <!-- Logo (Right) -->
      <div class="navbar-left">
        <NuxtLink to="/">
          <img src="~/assets/logo.jpeg
          " alt="Logo" class="logo" />
        </NuxtLink>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      isMenuOpen: false
    }
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    }
  }
}
</script>

<style scoped>
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: rebeccapurple;
  color: white;
  padding: 1rem;
}

.container {
  display: flex;
  justify-content: space-between;
  width: 100%;
  max-width: 1200px;
  margin: 0 auto;
}

.navbar-left {
  flex: 1;
}

.search-bar {
  padding: 0.5rem;
  border-radius: 4px;
  border: none;
  max-width: 200px;
}

.navbar-center {
  flex: 2;
  display: flex;
  justify-content: center;
  position: relative;
}

.toggle-button {
  background-color: transparent;
  color: white;
  border: none;
  font-size: 1.2rem;
  cursor: pointer;
}

.collapsing-menu {
  position: absolute;
  top: 100%;
  background-color: #444;
  padding: 0.5rem;
  border-radius: 5px;
}

.collapsing-menu .navbar-item {
  display: block;
  padding: 0.5rem;
  color: white;
  text-decoration: none;
}

.collapsing-menu .navbar-item:hover {
  background-color: #555;
}

.navbar-right {
  flex: 1;
  display: flex;
  justify-content: flex-end;
}

.logo {
  height: 50px;
}
</style>
