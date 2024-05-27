<template>
    <div>
      <Navbar />
      <div class="container mt-5">
        <Carousel />
        <div class="row mt-5">
          <Card v-for="(product, index) in products" :key="index" :product="product" />
        </div>
      </div>
      <Footer />
    </div>
  </template>
  
  <script>
  import Navbar from './components/Navbar.vue';
  import Carousel from './components/Carouse1.vue';
  import Card from './components/Card.vue';
  import Footer from './components/Footer.vue';
  
  export default {
    name: 'App',
    components: {
      Navbar,
      Carousel,
      Card,
      Footer
    },
    data() {
      return {
        products: [
          { id: 1, name: 'Product 1', price: 100, image: 'https://via.placeholder.com/150' },
          { id: 2, name: 'Product 2', price: 150, image: 'https://via.placeholder.com/150' },
          { id: 3, name: 'Product 3', price: 200, image: 'https://via.placeholder.com/150' },
          // Add more products as needed
        ]
      }
    }
  }
  </script>
