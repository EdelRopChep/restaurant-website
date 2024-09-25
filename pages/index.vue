<template>
 
  <section class="homepage">
    <div class="content">
      <!-- Text on the Left -->
      <div class="text-section">
        <i>
        <h1>Experience the Finest Chinese Cuisine in Nairobi</h1>
        <p>At Edan's, we serve authentic and delicious Chinese cuisine crafted from the freshest ingredients and inspired by timeless traditions</p>
       <b> <p>DINE WITH US.</p></b>
      </i>
      </div>

      <!-- Image on the Right -->
      <div class="image-section">
        <img src="~/assets/index.jpeg" alt="Sample Image" class="right-image" />
      </div>
    </div>
  </section>

   

  <section class="homepage">
    <div class="content flex items-center">
      <!-- Image on the Left -->
      <div class="image-section">
        <img src="~/assets/index1.jpeg" alt="Sample Image" class="left-image" />
      </div>

      <!-- Text on the Right -->
      <div class="text-section ml-5">
      <i> <h1>Founded by a passionate chef with roots in traditional Chinese cuisine, Edan’s aims to bring authentic flavors to Nairobi.</h1>
        <p>We believe in serving only the finest ingredients, sourced responsibly to create delightful dishes.</p>
        <b><p>VIEW MENU.</p></b></i> 
      </div>
    </div>
  </section>

  <section class="homepage">
    <div class="content">
      <!-- Text on the Left -->
      <div class="text-section">
        <i>
        <h1>Book your table in just a few clicks and guarantee your spot!</h1>
        <p>A world without food is horrible so book with us to experience love with our lovely meal.</p>
       <b> <p>BOOK A TABLE.</p></b>
      </i>
      </div>

      <!-- Image on the Right -->
      <div class="image-section">
        <img src="~/assets/index2.jpeg" alt="Sample Image" class="right-image" />
      </div>
    </div>
  </section>

   

  <section class="homepage">
    <div class="content flex items-center">
      <!-- Image on the Left -->
      <div class="image-section">
        <img src="~/assets/index3.jpeg" alt="Sample Image" class="left-image" />
      </div>

      <!-- Text on the Right -->
      <div class="text-section ml-5">
        <i><h1>Host your next celebration with us!</h1>
        <p> We offer personalized menus for special occasions.</p>
        <b><p>BOOK WITH US OR VIEW OUR MENU</p></b></i>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'HomePage'
}
</script>

<style scoped>
.homepage {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 2rem;
  background-color: lemonchiffon;
}

.content {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1200px;
  width: 100%;
}

.text-section {
  flex: 1;
  padding-right: 2rem;
}

.text-section h1 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
}

.text-section p {
  font-size: 1.2rem;
  margin-bottom: 1rem;
}

.image-section {
  flex: 1;
  text-align: right;
}

.right-image {
  max-width: 100%;
  height: 350px;
  border-radius: 8px;
}
.left-image {
  max-width: 100%;
  height: 350px;
  border-radius: 8px;
  }
  .text-section {
  margin-left: 30px; /* Space between image and text */
}
</style>
