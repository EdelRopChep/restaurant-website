<template>
  <div class="about-container">
    <i><h1>Welcome To Edan's Chines Restaurant.</h1>
    <p>
      Experience the Authentic Flavors of China.
      At Edan, we bring the vibrant tastes of traditional Chinese cuisine to your table. Our chefs craft each dish with fresh ingredients, time-honored techniques, and a passion for creating an unforgettable dining experience.
      From the spicy heat of Sichuan cuisine to the delicate flavors of Cantonese dim sum, our diverse menu offers something for every palate. Whether you’re craving crispy Peking Duck, savory Kung Pao Chicken, or a hearty bowl of Beef Noodle Soup, we invite you to savor the rich culinary heritage of China with every bite.
      Our Story
Inspired by the vibrant food markets of China, Edan was founded with the goal of sharing the authentic taste of Chinese cuisine with the local community. Our chefs draw from the diverse culinary regions of China, combining flavors that are both familiar and exotic to bring you a true taste of home.

We look forward to serving you soon! Come and discover the best of Chinese cuisine, right here in Nairobki!</p></i>
    </div>

  <div class="image-text-container">
    <div class="image-section">
      <img src="~/assets/about.jpeg" alt="Image Description" />
    </div>
    <div class="text-section">
     <i> <h2>WHY DINE WITH US?</h2></i>
      
     <p>Authentic Recipes: Every dish is prepared using authentic Chinese ingredients and recipes passed down through generations.</p>
       <p> Fresh Ingredients: We prioritize quality and freshness, ensuring that every bite bursts with flavor.</p>
          <p>Cozy Atmosphere: Our warm and inviting atmosphere is perfect for both intimate meals and group celebrations.</p>
             <p>Vegetarian & Vegan Options: We cater to all dietary preferences with a variety of vegetarian and vegan options that don’t compromise on taste.</p>
    </div>
  </div>
</template>

<script>
import Header from '~/components/Header.vue';
import Footer from '~/components/Footer.vue';
export default {
  name: "ImageText",
  head() {
    return {
      title: 'About Us',
    }
  }
}
</script>

<style scoped>
.about-container {
  background-color: lemonchiffon;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  padding: 20px;
}

h1 {
  margin-bottom: 20px;
}

p {
  font-size: 18px;
  line-height: 1.5;
}
.image-text-container {
  background-color: lemonchiffon;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 20px;
}

.image-section img {
  max-width: 100%;
  height: auto;
  border-radius: 10px;
}

.text-section {
  max-width: 50%;
  padding-left: 20px;
}

@media (max-width: 768px) {
  /* Make it stack vertically on smaller screens */
  .image-text-container {
    flex-direction: column;
    text-align: center;
  }

  .text-section {
    padding-left: 0;
    max-width: 100%;
  }

  .image-section {
    margin-bottom: 20px;
  }
}
</style>
